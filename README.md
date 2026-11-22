# Olivia's Gallery — Hugo source (yuzhi.win)

This branch holds the editable source for https://yuzhi.win.
The live site is published on the `master` branch by GitHub Actions
(see `.github/workflows/deploy.yml`).

## How to update the gallery
1. Add a photo to the right album folder under `content/`
   (e.g. `content/crafts/my-new-painting.jpg`), or create a new folder
   with an `index.md` for a new album.
2. Commit and push to the `source` branch.
3. GitHub Actions builds the site with Hugo and publishes it to `master`.

## Local preview
Install Hugo 0.140.2 extended, then run `hugo server` in this directory.

## Layout
- `hugo.toml` — site config (title, menus, outputs)
- `content/` — albums (page bundles: `index.md` + images) and pages
- `themes/gallery/` — the hugo-theme-gallery theme (vendored fork)
- `static/` — files copied verbatim to the published site (CNAME)
- `layouts/` — site overrides (analytics snippet in `partials/head-custom.html`)
