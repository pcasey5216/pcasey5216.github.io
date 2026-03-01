# Cost Analysis Interactive Labs

A collection of browser-based, single-file HTML tools for **training**, **intuition-building**, and **communicating assumptions** in cost-analysis contexts—no install required. Open the live links (or run locally) and start exploring. :contentReference[oaicite:3]{index=3}

## Live site (landing page)

- **Landing page:** https://pcasey5216.github.io/ :contentReference[oaicite:4]{index=4}

## Live tools (quick directory)

| Tool | What it’s for | Live link | Notes |
|---|---|---|---|
| **AI Bias Sandbox** | Rules-based sandbox for thinking through **bias exposure**, **traceability**, and **governance readiness** in AI/analytics workflows (DoD/ICEAA phrasing). :contentReference[oaicite:5]{index=5} | https://pcasey5216.github.io/AI_Bias_Sandbox.html | Scenarios stored locally in your browser (localStorage). :contentReference[oaicite:6]{index=6} |
| **Galton Board Distribution Lab** | Build distribution intuition (Galton board) and connect sampling to **cost PDF/CDF (S-curve)** results. :contentReference[oaicite:7]{index=7} | https://pcasey5216.github.io/Galton_Board_Distribution_Lab.html | Includes Monte Carlo + Latin Hypercube sampling options. :contentReference[oaicite:8]{index=8} |
| **K-Means Clustering Lab (v0.7.5.2)** | Interactive K-means explainer with step-through math, diagnostics, and exports—good for “t-shirt bucket” intuition. :contentReference[oaicite:9]{index=9} | https://pcasey5216.github.io/KMeans_Clustering_Lab.html | Teaching vs Analysis mode, elbow + silhouette helpers, CSV upload. :contentReference[oaicite:10]{index=10} |
| **CASE — Cost Analysis & Simulation Engine (v5.0.5)** | Build a WBS-driven estimate, add uncertainty + correlation + schedule phasing, run simulation, and export results. :contentReference[oaicite:11]{index=11} | https://pcasey5216.github.io/Cost_Analysis_Simulation_Engine.html | Includes tours + self-check (“Shift+Run”). :contentReference[oaicite:12]{index=12} |

---

# 1) AI Bias Sandbox (`AI_Bias_Sandbox.html`)

A **rules-based training sandbox** (not a statistical fairness score) for exploring how AI + analytics workflow choices can increase bias exposure and governance risk. :contentReference[oaicite:13]{index=13}

**Highlights**
- Guided “Start tour” + hover/tooltip definitions throughout. :contentReference[oaicite:14]{index=14}
- Inputs span lifecycle areas: use case, data/training, prompt/context, evaluation/monitoring, governance/use. :contentReference[oaicite:15]{index=15}
- Outputs update instantly (Exposure, Reliability, Governance readiness) with bias radar + drivers + mitigations. :contentReference[oaicite:16]{index=16}
- Save & compare scenarios (stored locally in browser). :contentReference[oaicite:17]{index=17}

**Suggested demos**
- Compare “Loose prompt / no eval” vs “RAG + red-team + HITL”
- Generate a “Model-Card / CARD addendum” style summary from a scenario :contentReference[oaicite:18]{index=18}

---

# 2) Galton Board Distribution Lab (`Galton_Board_Distribution_Lab.html`)

A visual lab that connects **Galton-board intuition** to sampling and cost-risk outputs (PDF + CDF / S-curve). :contentReference[oaicite:19]{index=19}

**Highlights**
- Drop balls to populate a Galton histogram; optionally simulate u-samples via MC or LHS. :contentReference[oaicite:20]{index=20}
- Choose a risk distribution (Normal, Lognormal, Triangular, Uniform, Weibull, Exponential). :contentReference[oaicite:21]{index=21}
- Map uncertainty to cost via direct / delta / multiplier modes and visualize the resulting PDF + CDF. :contentReference[oaicite:22]{index=22}

Tip: If canvases are blank, the header badge should indicate whether JS is loaded (e.g., “JS: OK”). :contentReference[oaicite:23]{index=23}

---

# 3) K-Means Clustering Lab (`KMeans_Clustering_Lab.html`) — v0.7.5.2

An interactive K-means sandbox: click to add points, step through iterations, and use diagnostics (elbow/silhouette) to pick **k**. :contentReference[oaicite:24]{index=24}

**Highlights**
- Teaching vs Analysis mode; k-means++ or random initialization; step / auto-run. :contentReference[oaicite:25]{index=25}
- CSV upload (choose columns, optional normalization) + repeatable presets via seed. :contentReference[oaicite:26]{index=26}
- Exports: points CSV + centroids CSV (includes cluster + t-shirt size fields). :contentReference[oaicite:27]{index=27}
- Built-in diagnostics: elbow + silhouette scan, convergence signals, cluster balance. :contentReference[oaicite:28]{index=28}

---

# 4) CASE — Cost Analysis & Simulation Engine (`Cost_Analysis_Simulation_Engine.html`) — v5.0.5

A browser-based estimating workflow: build a WBS-driven estimate, apply uncertainty, run simulation, and interpret results including percentiles and the S-curve. :contentReference[oaicite:29]{index=29}

**Highlights**
- Guided tours (quick start + end-to-end) and an in-app diagnostics/self-check (“Shift+Run”). :contentReference[oaicite:30]{index=30}
- Inputs support sampling approach (MC/LHS), base year vs then year output basis, correlation modes, and scenario save/load + import/export packages. :contentReference[oaicite:31]{index=31}
- Lines + WBS mapping + schedule phasing + risk configuration feeding results/interpretation. :contentReference[oaicite:32]{index=32}
- Planned-feature callouts exist in-app for items not implemented yet (e.g., risk register). :contentReference[oaicite:33]{index=33}

---

## What these tools are (and are not)

These tools are designed for **education, demos, and communicating assumptions**. They are **not validated pricing engines or compliance audit instruments**. :contentReference[oaicite:34]{index=34}

## Run locally

You can open each HTML file directly in a browser. For the most consistent behavior (especially if any browser restrictions affect local file access), run a tiny local server:

```bash
python -m http.server 8000
