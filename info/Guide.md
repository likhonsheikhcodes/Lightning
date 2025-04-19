# React Component Generation Guide

When generating a React component:

- Always use **TypeScript**; never use `any`.  
- Use **const** declarations instead of `function` for components.  
- Don’t annotate with `React.FC`; prefer explicit `JSX.Element` return types.  
- Compose components—adhere to React’s **composable pattern**.  
- Avoid overusing `useState`/`useEffect`; use **computed state**, `useMemo`, and `useCallback` to minimize renders.  
- Favor **server actions** + `useActionState` when possible; otherwise use `fetch` + API route handlers.  
  - For data mutations, accept server actions as props.  
- Prefer **Server Components**; fall back to Client Components only when needed.  
- Leverage **Suspense** and **streaming** for data loading.  
- Validate all inputs with **Zod** in server actions and API endpoints.  
- Encapsulate related state/effects in **custom hooks**.  
- Use **HOCs** for cross‑cutting concerns.  
- When logical, group related components, hooks, and utilities in the **same file**.  
- Always **HTML‑escape** text content.

---

## Recommended Libraries

1. **react-three-fiber** for 3D graphics  
2. **framer-motion** for animations  
3. **lodash** for utilities  
4. **react-confetti** for interactive effects  
5. **react-flow** for flow diagrams  
6. **react-bootstrap** for foundational UI

---

<!-- Coolors Palette Widget -->
<script src="https://coolors.co/palette-widget/widget.js"></script>
<script data-id="06086949665860586">
  new CoolorsPaletteWidget("06086949665860586", ["1a535c","4ecdc4","f7fff7","ff6b6b","ffe66d"]);
</script>

React and Next.js features, start prompt engineering with v0 today. v0’s ability to generate high‑quality UIs, leverage third‑party libraries, and provide detailed code breakdowns makes it an invaluable tool for frontend development—and everyone else surrounding the development workflow.
