# HeatWater — Heat & Water Vulnerability Intelligence

**Turning climate-risk indicators into actionable planning priorities.**

HeatWater is a climate-resilience decision-support prototype designed to help planners explore areas where extreme heat and limited water access may overlap. It combines a web-based vulnerability dashboard and resource-planning interface with an AI companion built using AWS PartyRock.

## 🚀 Project Links

- **Live Website:** https://deepikadawar.github.io/aws/
- **AI Companion — AWS PartyRock:** https://partyrock.aws/u/deepika68/bjuSpLj20/HeatWater-Risk-Explainer-for-Planners
- **GitHub Repository:** https://github.com/deepikadawar/aws

## 🌍 Problem Statement

Extreme heat and limited access to drinking water can create overlapping risks for outdoor workers and vulnerable communities. Planners may need to consider several factors simultaneously while deciding where to prioritize limited resources.

HeatWater explores how a simple digital platform can help users investigate these risks, compare illustrative vulnerability indicators, and consider potential interventions.

## 💡 Our Solution

HeatWater provides a unified entry point to climate-risk exploration and AI-assisted scenario analysis.

### 1. Vulnerability Dashboard
- Explore illustrative heat and water vulnerability indicators.
- Compare sample zones and identify areas flagged for further attention.
- Present risk information through a visual dashboard.

### 2. Resource Planner
- Explore how limited resources could be allocated across priority zones.
- Consider potential interventions, including drinking-water stations.
- Support preliminary planning through scenario exploration.

### 3. Methodology and Transparency
- Explain the project's approach and assumptions.
- Make the limitations of the prototype clear.
- Distinguish illustrative demonstration data from verified environmental measurements.

### 4. HeatWater AI — AWS PartyRock
- Explore user-provided heat-risk, water-access, and outdoor-worker-exposure scenarios.
- Generate AI-based explanations of potential risks.
- Suggest possible interventions, such as water access points, rest breaks, and safer outdoor work schedules.

The AI companion is a separate prototype accessible through the main website. It is not yet connected to the website through a shared backend.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Website hosting | GitHub Pages |
| AI companion | AWS PartyRock |
| Generative AI | PartyRock's AI application capabilities |
| Source control | GitHub |

## 🏗️ Architecture

The project currently consists of two separate components:

**Component A — Web Platform**
- Static website built with HTML, CSS, and JavaScript.
- Hosted on GitHub Pages.
- Provides the dashboard, planning interface, and methodology information.

**Component B — AI Companion**
- Built using AWS PartyRock.
- Accepts user-provided scenario information.
- Generates potential risk explanations and intervention suggestions.
- Accessible through a link on the main website.

The two components currently operate independently. The website does not send its dashboard data directly to the AI companion.

## ☁️ How We Used AWS

We used **AWS PartyRock** to create *HeatWater Risk Explainer for Planners*, an AI companion that helps users explore heat-and-water vulnerability scenarios.

PartyRock allowed us to prototype a generative AI experience without building and managing a separate AI-serving backend. We refined the interaction around user-provided scenario inputs and AI-generated
