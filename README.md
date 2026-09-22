# 2023-debt_climate_data

## About

Hosts a country-level dataset (Excel and CSV) combining debt distress risk (August 2022, IMF/World Bank Debt Sustainability Framework) with a climate vulnerability index (2020), alongside World Bank income classification and region, for reference and download.

Asset-hosting repo only — there is no page here, no `src/`, and the Webpack build tooling has been removed (see git history: "this is an asset-hosting repo, not a built site"). `public/` is synced directly to production.

## Rights of usage

Contact Teemo Tebest.

## Files and folders

* `public/assets/data/2023-debt_climate_data.xlsx` / `.csv` — the dataset, hosted as static files.

## Hosting

No build step — `npm run sync-prod` copies `public/*` directly to `https://storage.unctad.org/2023-debt_climate_data/` via `azcopy`; `npm run sync-gh-pages` mirrors `public/` to this repo's GitHub Pages branch.
