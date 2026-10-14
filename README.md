# Between the flags

FIT3179 Data Visualisation 2, Semester 2 2026. Author: Naman.

A single-page visualisation of drowning in Australia, with a focus on the NSW coast and Surf Life Saving.

## Structure
- `index.html`: the page
- `css/style.css`: layout and typography
- `specs/`: one Vega-Lite JSON file per chart
- `data/`: CSV and GeoJSON files, with sources in `data/README.md`

## Run locally
The specs load data with relative paths, so open the page through a local server rather than double-clicking it:

    python3 -m http.server 8000

Then visit http://localhost:8000.
