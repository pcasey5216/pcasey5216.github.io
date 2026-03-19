# Cost Analysis Interactive Labs

A collection of browser-based, single-file HTML tools for training, intuition-building, and communicating assumptions in cost-analysis contexts—no install required. Open the live links (or run locally) and start exploring.

## Live site

- Landing page: https://pcasey5216.github.io/

## Tools

| Tool | What it’s for | Live link |
|---|---|---|
| **AI Bias Sandbox** | Rules-based sandbox for thinking through bias exposure, traceability, and governance readiness in AI/analytics workflows. | https://pcasey5216.github.io/AI_Bias_Sandbox.html |
| **Galton Board Distribution Lab** | Build distribution intuition (Galton board) and connect sampling to PDF/CDF (S-curve) results. | https://pcasey5216.github.io/Galton_Board_Distribution_Lab.html |
| **K-Means Clustering Lab** | Interactive K-means explainer with diagnostics; great for “t-shirt bucket” intuition. | https://pcasey5216.github.io/KMeans_Clustering_Lab.html |
| **CARE — Cost Analysis Regression Engine** | Interactive regression lab for comparing model forms, transforms, fit quality, and minimization choices. | https://pcasey5216.github.io/CARE_Cost_Analysis_Regression_Engine.html |
| **CASE — Cost Analysis & Simulation Engine** | WBS-driven estimating workflow + uncertainty + correlation + phasing + simulation + exports. | https://pcasey5216.github.io/Cost_Analysis_Simulation_Engine.html |

---

## AI Bias Sandbox (`AI_Bias_Sandbox.html`)

A rules-based training sandbox (not a statistical fairness score) for exploring how AI + analytics workflow choices can increase bias exposure and governance risk.

**Highlights**
- Guided tour + tooltip definitions throughout
- Lifecycle inputs: use case, data/training, prompt/context, evaluation/monitoring, governance/use
- Outputs: exposure/reliability/governance readiness, key drivers, mitigations
- Save & compare scenarios (stored locally in your browser)

---

## Galton Board Distribution Lab (`Galton_Board_Distribution_Lab.html`)

A visual lab that connects Galton-board intuition to sampling and risk outputs (PDF + CDF / S-curve).

**Highlights**
- Drop balls to populate a histogram; optional Monte Carlo or Latin Hypercube sampling
- Common distributions (e.g., normal/lognormal/triangular/uniform/weibull/exponential)
- Visualize resulting PDF + CDF

---

## K-Means Clustering Lab (`KMeans_Clustering_Lab.html`)

An interactive K-means sandbox: add points, step through iterations, and use diagnostics (elbow/silhouette) to pick **k**.

**Highlights**
- Teaching vs analysis workflow
- Step / auto-run, initialization options, repeatability via seed (if enabled)
- Optional CSV upload and exports (if enabled)
- Diagnostics: elbow + silhouette-style helpers (if enabled)

---

## CARE — Cost Analysis Regression Engine (`CARE_Cost_Analysis_Regression_Engine.html`)

A browser-based regression lab for exploring candidate equations, transforms, fit metrics, and best-fit behavior across multiple model forms.

**Highlights**
- Guided tours + built-in diagnostics/self-check (if enabled)
- Compare regression forms, transforms, and best-fit candidates in one place
- Visualize data, trend lines, residual behavior, and fit-quality metrics
- Support training, demos, and estimator intuition-building around CER development

---

## CASE — Cost Analysis & Simulation Engine (`Cost_Analysis_Simulation_Engine.html`)

A browser-based estimating workflow: build a WBS-driven estimate, apply uncertainty, run simulation, and interpret results (including percentiles and the S-curve).

**Highlights**
- Guided tours + built-in diagnostics/self-check (if enabled)
- Inputs for sampling approach, base/then-year output basis, correlation modes, scenario save/load + export
- WBS mapping + schedule phasing + risk configuration feeding outputs

---

## What these tools are (and are not)

These tools are designed for education, demos, and communicating assumptions. They are not validated pricing engines or compliance audit instruments.

## Run locally

You can open each HTML file directly in a browser. For the most consistent behavior, run a tiny local server:

```bash
python -m http.server 8000
```
