# Nika Areshidze — Academic website

A lightweight, accessible academic website for Nika Areshidze, Ph.D. student in Mathematics at the University of California, Irvine.

## Contents

- Research interests and advisor information
- Eleven publications and preprints, with clickable titles
- Seven teaching assistant appointments at UC Irvine
- Talks and conferences
- Academic email and office information

All website files are in `dist/`. The site uses plain HTML and CSS, with no JavaScript, build step, package installation, external font service, analytics, or database. It uses the original portrait, biography, and Google Scholar link from the public Google homepage.

## Publish on GitHub Pages

The intended personal website repository is `nareshidze.github.io` under the GitHub account `nareshidze`.

1. Push this repository to GitHub on the `main` branch.
2. In the repository, open **Settings → Pages** and set **Source** to **GitHub Actions**.
3. Open **Actions → Publish academic website → Run workflow**, or push a new commit to `main`.

The included `.github/workflows/pages.yml` deploys `dist/` using GitHub's official Pages actions. After successful publication, the personal website will be available at `https://nareshidze.github.io/`.

The same source also works as a project site because all local asset paths are relative.

GitHub references:

- <https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages>
- <https://docs.github.com/en/pages/quickstart>

## Edit the website

| File | Purpose |
| --- | --- |
| `dist/index.html` | Biography, research, publication list, teaching, talks, and contact details |
| `dist/assets/style.css` | Colors, typography, desktop/mobile layouts, and print styling |
| `dist/assets/nika-areshidze.jpg` | Original portrait from the Google homepage |
| `dist/assets/favicon.svg` | Browser icon |
| `SOURCES.md` | Public sources used to verify the academic information |

To add a paper, duplicate an existing `li.paper` entry in `index.html` and give it a unique ID. Update its linked title, coauthors, year, and venue/status. The ordered list numbers the papers automatically.

An ahead-of-print journal article is included under Published and clearly labeled Ahead of print. Unpublished papers are labeled Preprint.

To add a CV later, put the file in `dist/assets/` and add a relative link in `index.html`. No placeholder CV is included. Update the year of study in the biography as needed.

## Local preview

Open `dist/index.html` directly in a browser, or run:

```sh
python3 -m http.server 8000 --directory dist
```

Then open `http://localhost:8000`. Click a paper's title to open its primary source.

## Accessibility and portability

The site includes semantic headings, a skip link, keyboard focus indicators, naturally wrapping navigation, a descriptive portrait alternative, responsive layouts, and a print stylesheet. All content and navigation work without JavaScript. No absolute `/assets/` paths or framework runtime are required.

Academic content was checked on November 3, 2026. Links lead to author preprints, journals, university pages, and the public academic homepage. See `SOURCES.md`.
