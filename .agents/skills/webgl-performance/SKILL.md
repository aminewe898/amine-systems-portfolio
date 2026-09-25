---
name: webgl-performance
description: Protect runtime performance and rendering quality for Three.js and React Three Fiber work in the Amine Systems Portfolio. Use for scenes, render loops, models, materials, particles, post-processing, textures, scroll-driven 3D, loading, and mobile fallbacks.
---

# WebGL Performance

Prioritize stable frame pacing over visual excess.

## React Three Fiber

Do not use React state for values that update every frame.

Use refs and mutate Three.js objects inside `useFrame` when appropriate.

Never instantiate expensive geometry/material objects repeatedly inside
the render loop.

Reuse resources.

Dispose custom resources correctly when they are no longer needed.

## Scene architecture

Prefer one coherent persistent Canvas/renderer architecture.

Avoid multiple expensive simultaneous WebGL renderers unless the design
requires them and profiling proves they are acceptable.

Pause or reduce work for scenes that are not visible.

Lazy-load expensive scene content.

## Geometry

Keep geometry appropriate for the actual viewing distance.

Use instancing for repeated meshes when beneficial.

Avoid absurd polygon counts for objects that occupy few screen pixels.

## Textures

Prefer compressed, web-appropriate textures.

Use 1K textures by default.

Use 2K only when visible quality justifies it.

Avoid unnecessary 4K+ textures.

Do not load textures the user is unlikely to see immediately.

## Models

Prefer GLB/glTF.

Optimize models before shipping when necessary.

Remove:
- unused geometry
- unused materials
- hidden objects
- unnecessary animation tracks
- excessive texture resolution

## Post-processing

Post-processing must be restrained.

Bloom should support emissive materials, not wash out the interface.

Use expensive effects only where visually justified.

Reduce or disable costly effects on weak devices.

## DPR

Do not blindly render at unrestricted devicePixelRatio.

Use a sensible cap and adapt rendering quality if performance drops.

## Performance adaptation

Use R3F/Drei performance tools where appropriate.

Possible quality tiers may alter:
- DPR
- shadows
- particles
- postprocessing
- model detail
- texture detail
- environmental effects

Do not make quality changes so aggressive that the design suddenly looks
broken.

## Scroll animation

Do not perform expensive DOM measurements every render frame when the
values can be cached or updated on resize/layout changes.

Keep GSAP/Lenis/R3F synchronization intentional.

Avoid multiple independent systems fighting over camera transforms.

## Profiling

Do not guess about performance.

Use:
- Chrome DevTools
- performance timeline
- GPU/render observations
- console warnings
- browser viewport testing

Check both desktop and mobile-sized viewports.

## Completion standard

A scene is not complete simply because it looks impressive on a powerful GPU.

It must also:
- remain responsive
- avoid unnecessary allocations
- avoid console warnings
- degrade gracefully
- respect reduced motion
- avoid blocking useful page content while assets load
