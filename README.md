# Oxford University Hospitals – First Seizure Referral simulatiion

This repo contains a single-file interactive webpage (`index.html`) for **service-planning estimates** of first seizure clinic referrals for Oxford University Hospitals.

## Features

- Incidence slider (20–100 per 100,000/year; defaults to 60 as a midpoint within the commonly cited 50–70 band)
- Catchment population set to **805,000**
- Toggle-able mimic categories:
  - Syncope (+25%)
  - Functional/dissociative attacks (+12%)
  - Panic/anxiety events (+6%)
  - TIA/migraine/other neuro mimics (+7%)
- Dark navy UI
- Oxfordshire boundary overlay (highlight) from GeoJSON (see Data Sources)

> The uplift percentages are **illustrative**. Tune these to your local audit data.

## Run locally

Just open `index.html` in a browser.

## Deploy on GitHub Pages

1. Upload `index.html` to the repo root.
2. Go to **Settings → Pages**
3. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
4. Save.

Your site will be available at:

`https://YOURUSERNAME.github.io/REPO/`

## Data sources

- Oxfordshire boundary (GeoJSON): `glynnbird/ukcountiesgeojson`  
  Raw file used by the page:  
  `https://raw.githubusercontent.com/glynnbird/ukcountiesgeojson/master/oxfordshire.geojson`

If your organisation has an official provider catchment GeoJSON for Oxford University Hospitals, you can swap the overlay to match the true catchment.

## Disclaimer

Planning / educational tool only. Not a clinical decision aid.
