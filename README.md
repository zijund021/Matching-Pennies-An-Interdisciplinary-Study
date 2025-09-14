# Matching Pennies: An Interdisciplinary Study

## Abstract
This study examines the game Matching Pennies (distinct from Prisoner’s Dilemma or Battle of the Sexes) using three methods: (i) theoretical predictions of Nash equilibrium in mixed strategies, (ii) human behavioral sessions, and (iii) interactions with a large language model (ChatGPT-5) under different prompt visibility conditions. Theoretical analysis shows a unique mixed equilibrium where both players randomize heads/tails with equal probability 0.5,0.5. Human subjects over seven rounds systematically deviate via streaks and heuristic patterns. The LLM reproduces heuristic behavior under “rule-only” visibility but aligns more closely with equilibrium when the payoff matrix is fully visible. I propose a refinement: a visibility-conditioned quantal-response type model to capture how presentation (visibility of payoffs) shifts behavior toward equilibrium.

## Task Summary
This project aims to explore strategic behavior in the Matching Pennies game using three lenses:

1️⃣Theory: Derive the equilibrium predictions for Matching Pennies (mixed strategy Nash equilibrium, uniqueness, zero-sum efficiency).

2️⃣Computation: Use Python tools (NashPy, QuantEcon) and Game Theory Explorer (GTE) to compute equilibria, verify payoff matrices, and illustrate extensive-form representations.

3️⃣Behavioral comparisons: Run experimental sessions with human participants and with an LLM (ChatGPT-5) under different visibility / prompt conditions. Observe how presentation of payoffs (rule-only vs full-matrix) affects strategy, randomness, and deviation from equilibrium.

The core hypothesis is that making payoff matrices explicit increases alignment with the equilibrium mix (closer to 50/50), whereas minimal presentation invites heuristic or pattern-based deviations.

## Reproduction Steps
1. See `economist/README.md`to get the basic knowledge about the game and the concepts.
2. Open `computational_scientist/ProblemSet_1_20250914.ipynb` and run all cells.
3. See GTE screenshots (with captions) in `computational_scientist/GTE.png,GTE,tex`.
4. Run the oTree app per `behavioral_scientist/README.md`.
5. Review LLM prompts/transcript in `behavioral_scientist/llm/`.


**PDF(overleaf):** https://www.overleaf.com/read/rcynmjvcddhf#3c75be

**Colab:** https://colab.research.google.com/drive/1S1s4Mx6FWe9G8UO_cvPr8hqMKhjjSIzN?usp=sharing)

