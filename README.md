# Bias Forecasting Sandbox (Cloud, CSP-Agnostic) — DoD/ICEAA Assumption-Driven Bias Dashboard

An interactive, educational dashboard for cost analysts to explore how common **CARD/BOE/IGCE assumption choices** can introduce **predictable bias exposure**—even when scope doesn’t change. This tool focuses on *bias mechanics and defensibility*, not “true pricing.”

## Live Demo
- (Add your GitHub Pages link here once enabled)

## What you can do
Adjust four assumption domains:
1. **Data Pedigree** (traceability, WBS/scope alignment, FY$ normalization, sample size, recency, missing/outliers, survivorship)
2. **Method Choices** (analogy/parametric/build-up blend, BOE maturity, cross-checks, reuse/learning, commitment posture)
3. **Economic & Rates** (contract context, escalation approach, rate stance, indirect handling)
4. **Schedule & Risk** (schedule realism, P50–P90 posture, correlation, uncertainty stance, risk register linkage, budget/anchor/competition pressure)

Outputs include:
- **Bias Risk Score (0–100)**
- **Traceability/Defensibility score (0–100)**
- **CARD readiness indicator**
- Likely **bias direction** (under/over/ambiguous)
- **Bias radar**, **drivers**, and **mitigation suggestions** (DoD/ICEAA language)
- Local **scenario save/compare**

## Files
- `index.html` — the dashboard (open in any modern browser)
- `qr.html` — paste your hosted URL to generate a QR code for slides

## Host this as a webpage (GitHub Pages)
1. Put `index.html` in the repo root (this repo).
2. Go to **Repo → Settings → Pages**
3. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main** (or master) / **root**
4. Save. Your site will publish to a URL like:
   - `https://<username>.github.io/<repo>/` (project site), or
   - `https://<username>.github.io/` (if using the special `<username>.github.io` repo)

## QR code for your presentation
After Pages is live:
1. Open `qr.html` locally
2. Paste the final hosted URL
3. Generate the QR and screenshot it into PowerPoint

## Disclaimer
This is a **rules-based educational tool** meant for training and discussion. The “cost” model is a lightweight placeholder to illustrate how bias and defensibility can shift results. It is not a validated pricing engine.
