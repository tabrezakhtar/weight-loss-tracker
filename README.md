# Weight‑Loss Tracker

<p align="center"><img src="https://www.tabrezakhtar.co.uk/assets/img/weightloss.png" alt="Weight-loss tracker screenshot" width="480" /></p>

A lightweight, privacy-first weight tracker built with **Astro** and modern ES6 JavaScript - perfect for logging progress, visualising trends, exporting CSVs, and sharing short, private links.


---

## Features

- Log and edit weight entries quickly (`WeightInput`, `WeightList`).
- Interactive trend `Graph` and summary stats.
- Export/import CSV and generate a short share link (`Csv.astro`, `GenerateLink.astro`).
- Local-first & privacy-minded: data is stored in the browser; no server required. See `privacy.md` for details.
- Tiny, dependency-light Astro frontend (mobile-first UI with Tailwind).


---

## Tech stack & conventions

- Framework: **Astro**
- Language: **ES6 JavaScript**
- Styling: **Tailwind CSS**
- UI: isolated Astro components in `src/components/`
- Data: browser localStorage / downloadable CSV


---

## Quick start - run locally

1. Clone the repo

   ```bash
   git clone <repo-url>
   cd weight-loss-tracker
   ```

2. Install

   ```bash
   npm install
   ```

3. Dev server

   ```bash
   npm run dev
   ```

4. Build for production

   ```bash
   npm run build
   npm run preview
   ```


---

## How to use (end‑user)

1. Open the app and enter your weight + date in `WeightInput`.
2. Toggle units in `Units` if needed; the app converts values.
3. View history in `WeightList` and trends in `Graph`.
4. Export your entries as CSV or generate a short link to share a snapshot.


---

## Project structure (key files)

- `src/pages/index.astro` - app entry (renders `Welcome`) 
- `src/components/Welcome.astro` - main UI container
- `src/components/WeightInput.astro` - add / edit entries
- `src/components/WeightList.astro` - list + delete entries
- `src/components/Graph.astro` - trend visualization
- `src/components/Csv.astro` - CSV export/import
- `src/layouts/Layout.astro` - global layout
- `public/` - static assets
- `tailwind.config.js` and `src/styles/global.css` - styling

---

## Contact / acknowledgements

- Built with Astro • Components live in `src/components/` • See `src/pages/contact.astro` to reach the maintainer.


---

Happy tracking!

