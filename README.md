# College-level Writing Dataset — project site

A static one-page site for the "College-level Writing Dataset" project
(NSF Tools Competition, Phase II). Plain HTML/CSS/JS — no build step,
so it hosts directly on GitHub Pages.

## Files
- `index.html` — page content
- `styles.css` — all styling
- `script.js` — mobile nav toggle

## Deploy to GitHub Pages

1. Create a new repository on GitHub (or use an existing one), e.g. `writing-dataset-site`.
2. Push these three files to the repo root:
   ```bash
   git init
   git add index.html styles.css script.js README.md
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub: go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   branch `main`, folder `/ (root)`. Save.
5. GitHub will publish the site at:
   `https://<your-username>.github.io/<repo-name>/`
   (takes a minute or two the first time).

## Editing content
All the copy — stats, comparison table, research questions, use cases,
PI names — lives directly in `index.html`. There's no CMS or data file;
edit the HTML in place and commit.

## Notes
- Fonts (Source Serif 4, Caveat) load from Google Fonts via `<link>` tags
  in `index.html` — no local font files needed.
- The layout is responsive down to mobile and respects
  `prefers-reduced-motion`.
