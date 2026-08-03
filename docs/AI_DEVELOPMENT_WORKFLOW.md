# AI Development Workflow

1. **Issue Parsing:** The AI reads the assigned GitHub Issue or task.
2. **Context Gathering:** Reviews `docs/ARCHITECTURE.md` and related source files in `src/js/` or `netlify/functions/`.
3. **Implementation:** Modifies vanilla JS, CSS, HTML, or Netlify functions as requested.
4. **Validation:** Runs `npm run build` to ensure the Vite build succeeds.
5. **Commit & PR:** Commits using Conventional Commits and opens a Pull Request using the appropriate template.
