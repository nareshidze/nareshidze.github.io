# Nika Areshidze — Academic website

Website: **https://nareshidze.github.io/**

A simple academic website for Nika Areshidze, Ph.D. student in Mathematics at the University of California, Irvine.

## Website files

- `index.html`: biography, papers, ongoing work, teaching, talks, and contact information
- `papers/`: PDFs of research drafts linked from the website
- `assets/style.css`: layout and typography
- `assets/nika-areshidze.jpg`: original portrait from the Google homepage
- `assets/favicon.svg`: browser icon
- `.nojekyll`: serves the website directly as static files
- `SOURCES.md`: academic content sources

## Publishing

GitHub Pages publishes this repository from the `main` branch and the `/(root)` folder. In **Settings → Pages**, the source is **Deploy from a branch**. Updates committed to `main` publish automatically.

No build command, package installation, or custom workflow is needed. The website uses plain HTML and CSS, with no application JavaScript, external font service, analytics, or database.

## Editing

Edit `index.html` to update the text and links. Each paper has one clickable title, followed by its coauthors and venue or preprint status. The profile links are Google Scholar, arXiv, and ResearchGate.

To add a paper, copy an existing `li.paper` entry, use a unique ID, and update the title link, coauthors, year, and venue. To update the portrait, replace `assets/nika-areshidze.jpg` and keep its image dimensions in `index.html` accurate.

Research drafts appear under **Ongoing work**, with a clickable title and a dated draft status. The Hardy draft was added on November 5, 2026.

All asset paths are relative. The layout works on desktop and mobile, with semantic headings, a skip link, keyboard focus styles, and print styling.

## Local preview

Open `index.html` in a browser, or run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

GitHub reference: <https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site>
