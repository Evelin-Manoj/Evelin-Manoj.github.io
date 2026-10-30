# Evelin Manoj — Portfolio

A single-file, dependency-free portfolio site built from the résumé.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole site: markup, styles and scripts in one file |
| `Evelin-Manoj-Resume.pdf` | Linked from the "Download résumé" button |
| `serve.js` | Tiny local static server for previewing (optional) |

## Preview locally

```bash
node serve.js . 8766
```

Then open <http://localhost:8766>. Double-clicking `index.html` also works, but the
résumé download link behaves best over HTTP.

## Publish for free

**GitHub Pages**
1. Create a repository (for example `evelin-manoj.github.io`).
2. Upload `index.html` and `Evelin-Manoj-Resume.pdf` to the root.
3. Settings → Pages → Source: *Deploy from a branch* → `main` / root.

**Netlify / Vercel**
Drag the folder onto the Netlify dashboard, or import the repository in Vercel. No build step is needed.

## Customise

- **Colours**: edit `--accent`, `--accent-2`, `--accent-3` at the top of the `<style>` block.
- **Typing phrases** in the hero: the `phrases` array near the bottom of the file.
- **Sections**: each `<section id="…">` is self-contained; remove or reorder freely and update the nav links to match.
- **Photo**: replace the `EM` monogram `<div class="avatar">` with an `<img>` if you want a headshot.
- **Theme**: a light/dark toggle is built in and remembered in `localStorage`.
