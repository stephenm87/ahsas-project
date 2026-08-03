# Deployment

## Production
- **Platform:** Netlify
- **URL:** https://ahsas-project.netlify.app
- **Build Command:** `npm run build`
- **Publish Directory:** `dist/`

## Continuous Integration
- GitHub Actions handles CI/CD through `build.yml`, `lighthouse.yml`, `preview.yml`, and `ci.yml`.
- Commits to `main` trigger a Netlify production build.
- Pull Requests trigger Netlify preview deployments.
