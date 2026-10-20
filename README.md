# Weihua Ma Academic Website

An independently designed static academic website for GitHub Pages. The project uses only HTML, CSS, and a small amount of JavaScript. It does not contain code, templates, Git history, or hidden content from the previous repository.

## Local preview

From this folder, run:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000/`.

## Content updates

- Biography, research interests, and education: edit `index.html` and the Chinese equivalents in `cn/index.html`.
- Conference papers, manuscripts under review, and works in progress: edit `publications/index.html`.
- Awards: edit `awards/index.html` and `cn/index.html`. Confirm official award and institution names before adding translations.
- Blog links or entries: edit `blogs/index.html`. Do not add post text unless it is publicly available and belongs to Weihua Ma.
- Profile details: the sidebar is repeated in each page so the site remains buildless. Search for `class="profile"` to update all copies.
- Visual design: edit `assets/css/style.css`.

## Updating the CV

1. Update the content near the bottom of `assets/cv/Weihua_Ma_CV.tex`; the reusable layout commands are defined at the top.
2. Compile it in Overleaf or with a local LaTeX installation. Latin Modern is declared in the source, so the typography remains consistent.
3. Replace `assets/cv/Weihua_Ma_CV.pdf` without changing the filename. The preview, download, and open buttons all point to this single file.
4. Open `/cv/` on desktop and mobile to verify the embedded preview and fallback links.

## GitHub Pages deployment

The site is published at <https://ma-weihua.github.io/> from the repository root of the `main` branch. GitHub Pages is configured to deploy from `/ (root)` with HTTPS enforced.

## Content provenance

The initial content inventory and translation notes are in `docs/content-audit.md` and `docs/award-revision-table.md`. The only reused media files are the portrait and WeChat QR code currently displayed on the public website.
