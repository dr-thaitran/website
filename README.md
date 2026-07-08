# Portfolio site — Quarto scaffold

A three-page Quarto site (Home / Research / Personal works) styled after the
visual-artist template, adapted to your world: gallery paper + ink palette,
Archivo Expanded display type, Newsreader serif body, and a documentary photo
grid that blooms from grayscale to colour on hover.

## Files
- `_quarto.yml` — site config + navbar (Home, Research, Personal works)
- `theme.scss` — the whole visual system (colours, type, hero, index, gallery)
- `head.html` — loads the fonts (Archivo, Archivo Expanded, Newsreader) from Google Fonts
- `index.qmd` — Home (bio-focused hero + about)
- `research.qmd` — papers, as an editorial index
- `personal.qmd` — photo projects + writings
- `images/` — placeholder portrait + 6 placeholder photos (replace these)

## Deploy via the GitHub web interface
1. In your repo, click **Add file → Upload files** and drag in every file above,
   keeping `images/` as a folder. (Or edit/replace your existing files.)
2. Commit. GitHub Pages rebuilds automatically if your repo already renders Quarto.
   If your repo publishes from `/docs` or a `gh-pages` branch, keep that setup — the
   `output-dir: _site` in `_quarto.yml` can be changed to `docs` to match.
3. If you preview locally: `quarto preview` from the project folder.

## Before it's "yours" — swap these placeholders
- **Portrait:** replace `images/portrait.jpg` with your real photo (portrait 4:5 works best).
- **Photos:** replace `images/photo-01…06.jpg`; update names/types/links in `personal.qmd`.
- **Papers:** in `research.qmd`, fix the third (placeholder) entry and add real DOI/PDF links.
- **Writings:** in `personal.qmd`, replace the three writing entries with real essays/videos.
- **Contact:** update the email (`you@example.com`) and GitHub URL in `_quarto.yml`,
  `index.qmd`, `research.qmd`, `personal.qmd`.

## Note on merging with your existing repo
This is a fresh scaffold. If your current repo already has a `_quarto.yml` (e.g. your
photos album-grid + lightbox), don't blind-overwrite it — copy the `navbar:` and
`theme:` lines across, or keep your album page and just link to it from `personal.qmd`.
