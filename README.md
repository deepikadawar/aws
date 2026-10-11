# HeatWater Vulnerability Intelligence

A hackathon MVP for the Heat & Water track. It demonstrates how a city team could combine heat intensity, water access, exposure, green cover, and service access to prioritize vulnerable zones and simulate where limited temporary water stations could be assigned.

## Important limitation

The built-in zone values are **illustrative demo data**, not live measurements, verified Delhi data, or an official public-health risk assessment. Do not use the prototype to make real-world emergency or public-health decisions. Before presenting claims about a real city, replace demo values with verified, dated, appropriately licensed datasets and document their sources.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Select zones, change the number of available stations, and click **Prioritize zones**.

No build tools, package installation, API key, or backend are required for this MVP.

## What it currently does

- Calculates a transparent weighted vulnerability score for each illustrative zone.
- Displays 12 clickable zones in a risk-colored grid.
- Shows a selected zone's factor scores and possible interventions.
- Ranks zones for a hypothetical temporary-water-station allocation.
- Lets the user vary station count and nominal capacity.

## Scoring model

Each input is normalized from 0–100. Water access, green cover, and service access are converted to gaps (`100 - input`).

`Vulnerability = 0.28 × heat + 0.25 × water_gap + 0.22 × exposure + 0.13 × green_gap + 0.12 × service_gap`

The allocation ranking is a separate heuristic:

`Priority = 0.55 × vulnerability + 0.20 × (population / 100) + 0.25 × water_gap`

These weights are prototype assumptions, not scientifically validated weights. They should be reviewed with domain experts and tested against suitable real data.

## AWS deployment idea

For a simple prize-eligible AWS deployment, host this static site on **AWS Amplify Hosting**. Connect the GitHub repository in the Amplify console and deploy the `main` branch. This gives the project a hosted URL. If the team chooses the AWS open-source-tool route instead, document the exact tool used and demonstrate it in the build; simply mentioning AWS in the README is not sufficient.

Potential later architecture (only add services you actually implement):
- Amazon S3: store versioned source datasets.
- AWS Lambda: ingest/transform new data and recalculate scores.
- Amazon DynamoDB: store zone features and computed outputs.
- Amplify Hosting: host the user interface.

Do not claim these services are used until they are genuinely integrated.

## Suggested next steps before final submission

1. Replace the sample values with verified datasets and show source date/licence in the UI.
2. Add a real geographic map only after obtaining valid coordinates and suitable map tiles/API terms.
3. Validate score weights with a local expert or publish them explicitly as a transparent screening heuristic.
4. Add a small test suite for score calculations and allocation ranking.
5. Record a 3-minute demo showing the problem, score explanation, changing station count, and limitations.
