# iceplant-report

Public hosting for **rendered Quarto reports** from the global iceplant
(*Carpobrotus*) occurrence project. Source code and data live in a separate
private repository; this repo holds only the published HTML for the team to
reference.

## Live site

Served via GitHub Pages: **https://king0708.github.io/iceplant-report/**

## Structure

```
.
├── .nojekyll        # disables Jekyll so Quarto asset folders (_files/, libs/) are served verbatim
├── index.html       # landing page linking to each report
├── README.md
└── reports/
    ├── global-occurrence.html   # Global iceplant (Carpobrotus) occurrence
    └── imagery-deepdive.html    # Regional imagery deep-dive (NZ · France · Portugal · Spain)
```

## Adding a report

1. Drop the rendered `.html` (self-contained / `embed-resources: true` preferred) into `reports/`.
2. Add a linked entry to `index.html`.
3. Commit and push to `main` — Pages redeploys automatically.

## Image credits

- Landing page photo: *Carpobrotus edulis 4* by
  [Lubman04](https://commons.wikimedia.org/wiki/File:Carpobrotus_edulis_4.JPG),
  licensed [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/),
  via Wikimedia Commons. Displayed unmodified. Stored at `assets/carpobrotus_edulis_lubman04.jpg`.

## Notes

- Reports are exported as self-contained HTML from Quarto, so all figures and
  data are embedded in each file.
- Files can be large (tens of MB); they are committed directly to git.
