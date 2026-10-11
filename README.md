# HeatWater — Vulnerability Intelligence

Responsive multi-page static website prototype.

## Pages
- `index.html` — landing page and project overview
- `dashboard.html` — clickable zone explorer, score indicators, searchable comparison table
- `planner.html` — adjustable station budget, ranked shortlist and CSV export
- `methodology.html` — formulas, proposed data pipeline and limitations
- `styles.css` — responsive visual system
- `app.js` — demo data and interactions

## Run locally
Open `index.html` in a browser. No package installation or API key is required.

## Publish with GitHub Pages
Upload all files to the repository root. Then open Settings → Pages, choose Deploy from a branch, select `main` and `/(root)`, and save.

## Important data notice
All 12 zones and their indicator/population values are simulated examples. They are not live Delhi data, official classifications, validated coefficients, or emergency warnings. The grid is conceptual, not geographically accurate. The planner is a simple ranking heuristic, not an optimized facility-location algorithm. Replace demo data with verified, licensed, timestamped data and validate the method with experts and communities before real-world use.

GitHub Pages hosts the static website but does not itself satisfy a separate requirement to use an AWS open-source tool. Do not claim AWS deployment or live data unless actually implemented and tested.
## AI Risk Explainer — AWS PartyRock

Try the companion AI prototype that explains combined heat, water-access, and outdoor-worker risks and suggests potential interventions.

[Open HeatWater Risk Explainer](https://partyrock.aws/u/deepika68/bjuSpLj20/HeatWater-Risk-Explainer-for-Planners)
