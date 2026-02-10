# Cost Analysis Interactive Labs

This GitHub Pages site hosts **two standalone, browser-based HTML tools** (no install, no build step).

## Live Tools

- **AI Bias Sandbox**  
  https://pcasey5216.github.io/AI_Bias_Sandbox.html

- **Galton Board Distribution Lab**  
  https://pcasey5216.github.io/Galton_Board_Distribution_Lab.html

---

## 1) AI Bias Sandbox (`AI_Bias_Sandbox.html`)

An interactive, **rules-based educational sandbox** for exploring how common AI + analytics choices can introduce bias risk across a workflow.

What you’ll find inside:
- A **Start Tour** walkthrough and in-page hover definitions (for terms and acronyms)
- Adjustable assumptions across typical lifecycle areas (use case, data, evaluation, governance)
- Real-time score/output updates as you change settings
- Scenario save/load behavior that runs locally in your browser

Note:
- This page is intended for **training / discussion / structured thinking**, not as a validated audit or compliance instrument.

---

## 2) Galton Board Distribution Lab (`Galton_Board_Distribution_Lab.html`)

A visual lab connecting **Galton board intuition** to **sampling** and **cost-risk charts**.

What you’ll find inside:
- Galton-board style sampling and distribution intuition
- Sampling modes (e.g., Monte Carlo / Latin Hypercube) and distribution options
- Cost-risk visualizations including **PDF** and **CDF (S-curve)** views
- A built-in **Tour** and hover definitions to explain how to use the tool

---

## Repo Files

- `AI_Bias_Sandbox.html`
- `Galton_Board_Distribution_Lab.html`
- `README.md`

(Optional but recommended)
- `index.html` (a simple landing page linking to both tools)

---

## Run Locally

You can open each file by double-clicking it.

For the most consistent behavior, run a tiny local server:

```bash
python -m http.server 8000
