# BREATHE Pelvic Health Center — website

Static, self-contained site ready for GitHub Pages.

## Deploy
1. Create a new GitHub repo (or use an existing one).
2. Upload the two files in this `gh-pages/` folder to the repo root:
   - `index.html` — the entire site (all pages, images, styles, and scripts inlined into one file)
   - `.nojekyll` — tells GitHub Pages to serve files as-is
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. Your site goes live at `https://<username>.github.io/<repo>/` within a minute or two.

## Notes
- `index.html` is fully offline-capable — no build step, no dependencies to install.
- The one thing that needs the internet at view time is the embedded Google **map** (it loads from maps.google.com) and Google **Fonts**. Everything else, including all photos, is inlined.
- Navigation between pages (Home / Why BREATHE / Specialties / Meet BREATHE / Blog) works via in-page routing — no extra files needed.

## Editing later
Don't hand-edit `index.html` (it's compiled). Edit the source `Breathe Website.dc.html` in the design tool, re-export, and replace `index.html`.
