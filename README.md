# Play to Innovate: An Interdisciplinary Approach from Game Theory to Mechanism Design in a Case Study

## 💕Acknowledgment
I am deeply grateful to **Professor Luyao Zhang** for generous guidance and high standards; her focused comments on writing, figures, software citations, and repository communication gave me clear direction and renewed confidence. I also thank **Runqi Li** for a thoughtful peer review that affirmed the balance between rigor and accessibility and encouraged a theory-to-application flow with ethical reflection. These affirming, actionable suggestions shaped the revisions below and materially improved the paper’s clarity, coherence, and usability.

## 👀Abstract  
- This two-part project connects classic game theory with modern computational and experimental tooling. 
- **Problem Set 1** selects **Matching Pennies** as the core environment and builds a full pipeline: formal analysis and welfare discussion; computational verification of equilibria using Nashpy and QuantEcon; an extensive-form rendering and SPNE check in Game Theory Explorer; and a lightweight experimental design in oTree with a human/LLM comparison. 
- **Problem Set 2** refines the write-up (figure titles, captions, cross-referencing, formal software citations) and extends into mechanism design by testing **an all-pay auction** with AI agents (GPT-5 Thinking, DeepSeek Thinking). We run a Control (known common value V=1000) and a Treatment (unknown V with private hints). In the control, bids show over-dissipation (total bids > prize value), consistent with aggressive play in all-pay settings. In the treatment, a single-shot trial with conservative bidding and tight, symmetric hints does not display winner’s-curse overpayment; we outline minimal tweaks (wider/bias signals, multiple rounds) to surface it. 
- All prompts, logs, and figures are included for reproducibility, and the repo documents how each tool supports analysis, computation, and experimental deployment. See tool references for Nashpy, GTE, oTree, QuantEcon, and classic winner’s-curse results.
- Payoff Matrix
<img width="1000" height="500" alt="1" src="https://github.com/user-attachments/assets/a3050c4d-7625-4500-9650-ac2d9eaa919b" />

- GTE Extensive Form
<img width="1000" height="500" alt="6" src="https://github.com/user-attachments/assets/06dc206b-878f-4673-91f7-685c820f256d" />

- LLM_Choice_and_Reason in game
<img width="1000" height="500" alt="1choice reason" src="https://github.com/user-attachments/assets/07bc59e0-e18f-448e-991c-ba4373e81e96" />

- LLM_Choice_and_Reason in auction
<img width="832" height="441" alt="C_GPT5" src="https://github.com/user-attachments/assets/9e85f4a6-3575-4751-9767-e6308fbca72f" />


## 🔧Tools/Platforms you need:
- Nashpy (Python)
- QuantEcon
- Game Theory Explorer (GTE)
- oTree
- Colab
- LLMs as agents — GPT-5 Thinking and DeepSeek Thinking
- Overleaf
- GitHub

## 📖Task Summary  
This project explores strategic behavior in **Matching Pennies and an auction design** across three lenses:

1. **Theory** – Derive the mixed-strategy Nash equilibrium, show uniqueness, and analyze efficiency/fairness in the zero-sum context.  
2. **Computation + Visualization** – Use Python (NashPy, QuantEcon) and GTE to compute equilibria, verify payoff matrices, and build extensive-form & strategic-form representations.  
3. **Behavior + Prompting** – Conduct sessions with human participants and with ChatGPT-5 under two visibility conditions (rule-only vs full-matrix), observe how showing payoff structure influences randomness, heuristic deviations, and alignment with equilibrium.
4. **All-Pay Auction with AI Agents** – Two-bidder, one-shot, first-price all-pay auction (highest bid wins; everyone pays own bid).



## 🪜Reproduction Steps  
1. Review theory + welfare in `economist/README.md`.  
2. In `computational_scientist/`, open `ProblemSet_1_20250914.ipynb` (Colab export) and run all cells.  
3. View GTE screenshots and settings in `computational_scientist/gte/` (tree + solver).  
4. Navigate to `behavioral_scientist/README.md` and deploy/run the oTree app.  
5. Examine LLM session artifacts in `behavioral_scientist/llm/` (prompts, transcript, settings.json) and human session screenshots.
6. Check `mechanism_design/`for auction design and outcomes.

---

## 🎺Point-by-Point Response
1. **Writing and Figure Presentation**，I revised：Standardized figure titles, captions, and cross-references; e.g., renamed Fig. 1 to Payoff matrix for Matching Pennies with \label{fig:mp-bimatrix}; merged former Figs. 2–5 into a 2×2 panel as Fig. 2 (Solver outputs confirming theory, \label{fig:mp-solvers}); combined the GTE tree and equilibrium into Fig. 3 (a–b) with labels \label{fig:gte-tree}, \label{fig:gte-solver},and panel \label{fig:gte-panels}.
2. **Software Citations**，I revised：Appended a Chicago-style References block in the manuscript and mirrored it at the bottom of the root README.md (Nashpy, GTE, QuantEcon, oTree), with DOIs/URLs and access dates.
3. **GitHub Enhancements**，I revised：Updated the root README.md: added Overview (purpose, tools), a Quick Start (env setup, run commands, reproduction notes), and a Key Figures gallery with embedded screenshots and one-sentence captions; included a short citation block at the end.

---
### 🐱References 
- Baye, Michael R., Dan Kovenock, and Casper G. de Vries. 1996. “The All-Pay Auction with Complete Information.” Economic Theory 8 (2): 291–305. \url{https://doi.org/10.1007/BF01211819}
- Camerer, Colin F. 2003. *Behavioral Game Theory: Experiments in Strategic Interaction*. Princeton, NJ: Princeton University Press.
- Chen, Daniel L., Martin Schonger, and Chris Wickens. 2016. “oTree—An Open-Source Platform for Laboratory, Online, and Field Experiments.” *Journal of Behavioral and Experimental Finance* 9: 88–97. https://doi.org/10.1016/j.jbef.2015.12.001.
- Kagel, John H., and Dan Levin. 1986. “The Winner’s Curse and Public Information in Common Value Auctions.” American Economic Review 76 (5): 894–920.
- Knight, Vincent. 2021. *Nashpy: A Python Library for the Computation of Equilibria of 2-Player Strategic Games*, Version 0.0.28. Documentation. https://nashpy.readthedocs.io/en/v0.0.28/.
- Nash, John F. 1951. “Non-Cooperative Games.” *Annals of Mathematics* 54 (2): 286–295.
- Osborne, Martin J. 2003. *An Introduction to Game Theory*. New York: Oxford University Press.
- Savani, Rahul, and Bernhard von Stengel. 2015. “Game Theory Explorer—Software for the Applied Game Theorist.” *Computational Management Science* 12: 5–33.
- Sargent, Thomas J., and John Stachurski. 2021. *Quantitative Economics with Python*, Version 0.5.1. Online book. https://python.quantecon.org/.
