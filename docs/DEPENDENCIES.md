# Dependencies

## Policy

Target additional monetary cost: **€0**.

Before introducing a significant dependency:

1. Confirm it solves a real requirement.
2. Check whether the existing stack already solves the problem.
3. Verify the required functionality is available without payment.
4. Check current compatibility with the project stack.
5. Run `npm audit`.
6. Run lint and production build.
7. Record the dependency here.

Do not use `npm audit fix --force` without first inspecting the proposed
dependency changes.

## Approved runtime stack

- Next.js
- React
- TypeScript
- Tailwind CSS
- Three.js
- React Three Fiber
- Drei
- React Postprocessing
- postprocessing
- GSAP
- Lenis
- Motion
- Zustand
- Howler

## Approved development tooling

- Leva
- Blender
- Context7 MCP free usage
- Motion documentation MCP
- OpenAI Developer Docs MCP
- Playwright MCP
- Chrome DevTools MCP

## Deliberately excluded

- r3f-perf
- gltfjsx as a project dependency
- Motion+
- paid animation plugins/services
- paid asset libraries
- paid fonts
- paid APIs

## Dependency changes

Record future additions here with:
- package/tool
- purpose
- source
- license/cost status
- reason existing tools were insufficient
