# Play to Innovate: An Interdisciplinary Approach from Game Theory to Mechanism Design

> **Abstract.**  
> This project connects classic game theory with modern computation and behavioral testing.  
> Part 1 formalizes strategic games (Matching Pennies), proves the mixed-strategy equilibrium, and evaluates efficiency/fairness with reproducible computation and extensive-form checks.  
> Part 2 extends to **mechanism design** via a two-bidder **first-price all-pay auction**, testing winner’s-curse claims on LLM agents under control vs. private-hints treatments.  
> All code, prompts, and figures are organized for review and replication.

---

## Authors & Roles
- **Zijun Ding** — *Economist; Computational Scientist; Behavioral Scientist; Mechanism Designer*  
  (lead on theory, code, experimental design, and write-up)

---

## Disclaimer
This repository supports the **final research proposal** submitted to **COMSCI/ECON 206: Computational Microeconomics**, instructed by **Prof. Luyao Zhang** at **Duke Kunshan University** in **Autumn 2025**.

---

## Acknowledgments
- **Faculty & peers.** Prof. Luyao Zhang for guidance; peer reviewers **Runqi Li** and **Ky Boughton** for constructive feedback.  
- **LLM agents.** GPT-5 Thinking; DeepSeek Thinking.  
- **Open-source communities.** **Nashpy**, **QuantEcon**, **Game Theory Explorer (GTE)**, **oTree**, **Matplotlib**, **Jupyter/Colab**, **LaTeX/Overleaf**, and **GitHub**.

---

## Statement of Growth
Across PS1 (strategic games), PS2 (mechanism design & auctions), and classroom collaborations, I:
- **Strengthened theory → computation → behavior** flow: clear assumptions & equilibrium concepts; verified with Python (Nashpy/QuantEcon) and GTE; deployed lightweight human/LLM sessions.
- **Improved research hygiene:** figure titling, captions, cross-referencing; formal software citations; repository navigation and communication.
- **Expanded design perspective:** built and evaluated minimal mechanisms (e.g., all-pay auction) and analyzed information salience (matrix visibility) on agent behavior.
- **Deepened professional skills:** collaborative review, reproducible pipelines, and ethically aware write-ups aligned with SDG-oriented impact.

---

## Table of Contents
- [`economist/`](./economist/) — Theory notes, welfare & fairness analysis, formatted figures. :contentReference[oaicite:3]{index=3}  
- [`computational_scientist/`](./computational_scientist/) — Notebooks & scripts (Nashpy/QuantEcon), GTE artifacts. :contentReference[oaicite:4]{index=4}  
- [`behavioral_scientist/`](./behavioral_scientist/) — Human & LLM sessions (oTree setup, prompts, logs). :contentReference[oaicite:5]{index=5}  
- [`mechanism_design/`](./mechanism_design/) — Auction design (control/treatment), prompts, outcomes. :contentReference[oaicite:6]{index=6}  
- [`visualizations/`](./visualizations/) — Key images & plots. :contentReference[oaicite:7]{index=7}  
- [`docs/`](./docs/) — Final PDF/LaTeX, poster, field-trip reflection. :contentReference[oaicite:8]{index=8}  

> Tip: This README follows GitHub’s guidance on repository docs—lead with purpose, then give scannable navigation and links. :contentReference[oaicite:9]{index=9}

---

## Navigation Instructions

### 1) Equilibria computation (PS1)
- **Normal form & mixed NE:** see `computational_scientist/` notebooks (Nashpy) and `economist/` derivations.  
- **Extensive form & SPNE:** see `computational_scientist/gte/` screenshots/settings and notes in `economist/`.  
- **Key figures:** payoff matrix & solver panels in `visualizations/`.

### 2) Mechanism design & simulations (PS2)
- **Auction prompts & runs:** `mechanism_design/` (Control: known \(V=1000\); Treatment: private hints).  
- **Outputs:** bids, dissipation, and brief interpretations per run.  
- **How to reproduce:** run prompt scripts or replay LLM logs; extend by varying hint dispersion/bidders.

### 3) Visualizations & outputs
- PNGs/SVGs in `visualizations/`. Link back from report sections via relative paths.

### 4) Documentation
- **Final report & LaTeX:** `docs/`  
- **Poster:** `docs/poster.*` (PDF/PNG)  
- **Field trip reflection:** `docs/field_trip.*`

> For reviewers: each folder begins with a short README or index where applicable, to reduce hunting for files.

---

## Quick Start (Reproducibility)
1. **Clone** the repo and open `computational_scientist/` notebooks in Jupyter/Colab.  
2. **Install** Python deps (see notebook headers).  
3. **Run** all cells to regenerate payoff matrices, solver checks, and figures.  
4. **Browse** `behavioral_scientist/` for oTree setup and LLM/human session logs; use provided prompts for replication.  
5. **Review** `mechanism_design/` for control vs. treatment runs; adjust parameters (hint width, tie-break seeds) to stress-test winner’s-curse dynamics.

---

## Embedded Media
- **Poster (PNG/PDF).**  
  ![Project Poster](./docs/poster.png "Poster")  
  > If your poster lives elsewhere (e.g., Canva), include a public link here as well.

---

## Citation & Software Credits
Please cite the tools used (Nashpy, QuantEcon, GTE, oTree, etc.) as listed in the paper’s References.

---

## License
[MIT](./LICENSE)
