# Implementation

## Milestone 0 — Foundation

Status: complete

Completed:
- Next.js project created
- TypeScript configured
- Tailwind configured
- Git repository initialized
- GitHub remote created
- clean baseline committed
- Three.js stack installed
- animation stack installed
- audio stack installed
- state tooling installed
- WebGL post-processing installed
- Leva development tooling installed
- npm audit clean
- lint clean
- production build clean
- Context7 MCP tested
- Motion MCP tested
- OpenAI Developer Docs MCP tested
- Playwright MCP tested
- Chrome DevTools MCP tested
- Blender available locally
- repository art-direction skill created
- repository WebGL-performance skill created
- zero-cost dependency policy established
- external asset policy established

## Milestone 1 — Vertical slice

Not started.

Target:
- navigation shell
- boot sequence
- global WebGL architecture
- hero
- Amine Core prototype
- first automation/n8n project scene
- basic audio manager
- sound toggle
- performance adaptation
- responsive fallback
- reduced-motion behavior

## Architecture decisions

### Rendering

Use a persistent/global React Three Fiber architecture unless profiling or
specific design requirements justify another approach.

### Animation ownership

GSAP:
- cinematic sequences
- ScrollTrigger
- WebGL camera timelines
- scene choreography

Motion:
- DOM interactions
- hover/tap feedback
- menus
- layout transitions

### Cost

Required project cost beyond already-owned hardware/services: €0.

## Open questions

- final open-source font pairing
- final sound-design workflow
- final Amine Core model design
- production hosting/deployment configuration

## Performance issues

None recorded yet.

## Asset requirements

Milestone 1 initially uses procedural geometry where practical.

Custom production 3D assets can replace prototypes after interaction,
lighting and camera direction are validated.
