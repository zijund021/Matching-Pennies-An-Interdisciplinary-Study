# Matching Pennies: An Interdisciplinary Study

## Abstract  
This study examines the game Matching Pennies (distinct from Prisoner’s Dilemma or Battle of the Sexes) using three methods: (i) theoretical predictions of Nash equilibrium in mixed strategies; (ii) human behavioral sessions; and (iii) interactions with a large language model (ChatGPT-5) under different prompt visibility conditions. Theoretical analysis shows a unique mixed equilibrium where both players randomize heads/tails with equal probability (0.5, 0.5). Human subjects over seven rounds deviate by streaks and heuristic patterns. The LLM behaves heuristically under “rule-only” visibility but aligns more closely with equilibrium when the payoff matrix is visible. I propose a refinement: a visibility-conditioned quantal-response model to capture how presentation of payoffs shifts behavior toward equilibrium.

## Task Summary  
This project explores strategic behavior in Matching Pennies across three lenses:

1. **Theory** – Derive the mixed-strategy Nash equilibrium, show uniqueness, and analyze efficiency/fairness in the zero-sum context.  
2. **Computation + Visualization** – Use Python (NashPy, QuantEcon) and GTE to compute equilibria, verify payoff matrices, and build extensive-form & strategic-form representations.  
3. **Behavior + Prompting** – Conduct sessions with human participants and with ChatGPT-5 under two visibility conditions (rule-only vs full-matrix), observe how showing payoff structure influences randomness, heuristic deviations, and alignment with equilibrium.

Core hypothesis: explicit payoff visibility leads to behavior closer to the theoretical 0.5/0.5 mixing; minimal prompt visibility yields more heuristic/pattern-based deviations.

## Reproduction Steps  
1. Review theory + welfare in `economist/README.md`.  
2. In `computational_scientist/`, open `ProblemSet_1_20250914.ipynb` (Colab export) and run all cells.  
3. View GTE screenshots and settings in `computational_scientist/gte/` (tree + solver).  
4. Navigate to `behavioral_scientist/README.md` and deploy/run the oTree app.  
5. Examine LLM session artifacts in `behavioral_scientist/llm/` (prompts, transcript, settings.json) and human session screenshots.  

---

## Repository Structure 
- `README.md` — title, abstract, task summary, reproduction steps  
- `economist/` — theory + welfare analysis; `refs/` holds PDFs/BibTeX or links  
- `computational_scientist/` — Colab-exported notebook; README with how-to-run & GTE exports/screenshots  
- `behavioral_scientist/` — oTree app; screenshots (game pages & session results); `llm/` (prompts, transcript, settings); README with deployment, session config, ethics

---

## Attribution & License  
This project uses tools such as oTree, NashPy, QuantEcon, etc. Please cite as appropriate. Licensed under the MIT License.  


