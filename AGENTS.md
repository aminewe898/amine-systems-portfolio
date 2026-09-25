<!-- BEGIN:nextjs-agent-rules -->

# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->

<!-- BEGIN:amine-portfolio-rules -->

# Amine Systems Portfolio

## Project goal

This repository is a premium interactive technical portfolio for
Mohamed Amine Aslimani focused on systems, networks, infrastructure,
automation, AI, hardware, and engineering work.

The site must feel like a designed technical experience rather than a
generic developer portfolio or AI-generated landing page.

## Core stack

Use the dependencies already installed in package.json.

Primary responsibilities:

- Next.js + React + TypeScript: application structure and semantic UI
- Three.js + React Three Fiber + Drei: WebGL and 3D
- GSAP + ScrollTrigger: cinematic and scroll-driven sequences
- Motion: DOM/UI microinteractions
- Lenis: smooth scrolling
- Zustand: experience state
- Howler: audio playback
- React Postprocessing: restrained 3D post-processing
- Leva: development-only visual tuning

Do not add a dependency when the existing stack can reasonably solve the task.

## Mandatory local skills

Use `$portfolio-art-direction` when implementing or reviewing:
- visual design
- page composition
- typography
- UI
- WebGL scenes
- 3D object presentation
- animation feel
- sound/interaction feel

Use `$webgl-performance` when implementing or reviewing:
- React Three Fiber
- Three.js
- shaders
- models
- textures
- particles
- render loops
- post-processing
- scroll-driven WebGL
- performance-sensitive animation

Use both when a task touches both visual design and WebGL implementation.

## Zero-cost policy

The project must remain buildable, developable and deployable without
requiring purchases.

Do not introduce:
- paid APIs
- paid fonts
- paid asset packs
- paid templates
- paid 3D models
- paid sound libraries
- subscription-only development tools
- Motion+ requirements
- premium shader packs
- paid hosting requirements

Free trials do not count as free.

Before adding an external dependency or asset, verify that the required
usage is available at no cost and record it in the appropriate docs file.

## External assets

Prefer:
1. original assets made for this project
2. CC0 assets
3. permissively licensed open-source assets

Record third-party visual/audio assets in `docs/ASSETS.md`.

Do not download random models, fonts, images or sounds without checking
their license.

## Design constraints

Do not drift toward generic AI/SaaS aesthetics.

Avoid:
- purple gradient backgrounds
- giant blurred gradient blobs
- meaningless floating spheres
- excessive glass cards
- shadcn-style card grids
- excessive pills
- rainbow neon
- fake hacker clutter
- arbitrary skill percentage bars
- animation that exists only to show off

Prefer:
- graphite and near-black surfaces
- black anodized aluminium
- gunmetal
- brushed silver
- restrained cobalt/electric-blue accents
- strong typography
- technical diagrams
- physical depth
- premium product lighting
- purposeful 3D
- restrained sound design

## Architecture rules

Keep semantic content in the DOM.

Use one persistent/global WebGL architecture rather than creating many
unrelated Canvas instances unless there is a justified technical reason.

GSAP owns cinematic timelines, scroll choreography and WebGL camera/object
sequences.

Motion owns DOM microinteractions, menu transitions, buttons and layout
animation.

Do not make GSAP and Motion compete over the same animated property.

Avoid React state updates every frame.

Do not create new Three.js geometries, materials or heavy objects inside
render loops.

Prefer refs and Three.js mutation for per-frame object updates.

Respect `prefers-reduced-motion`.

Provide graceful mobile/low-power fallbacks.

## Documentation

Update:
- `docs/IMPLEMENTATION.md` for architecture decisions and milestone progress
- `docs/DEPENDENCIES.md` when adding/removing significant dependencies
- `docs/ASSETS.md` when adding external assets

## Verification

For meaningful code changes run:

npm run lint
npm run build

For visual/interactive changes also inspect the running site using
Playwright and/or Chrome DevTools MCP.

Do not declare visual work complete based only on successful compilation.

Check:
- desktop rendering
- mobile viewport
- console errors
- keyboard usability
- reduced-motion behavior
- obvious performance regressions

<!-- END:amine-portfolio-rules -->
