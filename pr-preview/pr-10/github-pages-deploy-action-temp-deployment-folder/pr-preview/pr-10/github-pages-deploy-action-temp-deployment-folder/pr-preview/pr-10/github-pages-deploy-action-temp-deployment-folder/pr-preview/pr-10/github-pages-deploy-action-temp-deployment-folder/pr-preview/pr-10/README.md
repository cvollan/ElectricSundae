# Electric Sundae

One-page marketing site for [Electric Sundae](https://electric-sundae.com/), an event ice cream cart.

## Files

- `index.html` — the whole page (the inline script sets the footer year and flips flavor descriptions below their card when they'd run off the top of the viewport)
- `styles.css` — all styling; no framework
- `logo_long.webp`, `logo_small.webp`, `logo_long_stacked.webp` — logos

## Deployment (GitHub Pages)

- **Production** — `.github/workflows/pages-deploy.yml`: pushing to `main` (or running it manually via *Actions → Deploy production site → Run workflow*) deploys the repo to the `gh-pages` branch, served at `electric-sundae.com`.
- **PR previews** — `.github/workflows/pr-preview.yml`: every PR (including updates, and removal on close) is deployed via `rossjrw/pr-preview-action` to `gh-pages/pr-preview/<branch>/` and a preview URL is posted in the PR. The production deploy uses `clean-exclude: pr-preview/` so previews survive production deploys.
