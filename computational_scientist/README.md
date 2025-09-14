# Computational Scientist (normal form + GTE)

This folder contains the Colab notebook and GTE exports used to compute and visualize the mixed Nash equilibrium for Matching Pennies.

## Contents
- `ProblemSet_1_20250914.ipynb` — Colab-exported Jupyter notebook.    
- `GTE.png` `GTE.tex`— (optional) GTE export images/graphics.  

## How to Create Matching Pennies in GTE

This section explains step-by-step how to build the extensive-form + strategic-form representation of Matching Pennies in Game Theory Explorer (GTE).

---

### Step-by-step instructions

1. Open the GTE web app in your browser via the GTE homepage.  
   (Savani & von Stengel 2015 explain that GTE is designed to allow interactive creation of games in extensive or strategic form and solving Nash equilibria in the browser.) :contentReference[oaicite:0]{index=0}

2. Start a new game.

3. Build the extensive-form tree:
   - Create a root decision node for Player 1 with two branches/actions: `H` and `T`.
   - Under each of Player 1’s branches, create a decision node for Player 2.
   - Create an information set connecting Player 2’s two decision nodes (this models simultaneity: Player 2 does not know which node when choosing).

4. Assign payoffs at each terminal node to match the strategic-form payoff matrix:

5. If GTE shows a strategic-form matrix view (often on the side), check that it matches the same payoff matrix.

6. Solve for equilibrium:
- Use the solver tool (SPNE or Nash equilibrium tool) in GTE to compute the mixed equilibrium.
- Record solver output screenshot.

7. Export visuals:
- Export the extensive-form tree + strategic-form matrix screenshot.
- Export solver output screenshot.
- Save images in `gte/` folder with filenames like `6_gte_tree_and_matrix.png`, `7_gte_solver_output.png`.
<img width="1035" height="582" alt="6" src="https://github.com/user-attachments/assets/9aea132b-58b5-4354-849b-dd46e8de2608" />
<img width="774" height="486" alt="7" src="https://github.com/user-attachments/assets/428b94aa-9526-4284-8a65-08726103efc9" />

---

### Citation for GTE

- Savani, Rahul, and Bernhard von Stengel. 2015. “Game Theory Explorer — Software for the Applied Game Theorist.” *Computational Management Science* 12: 5-33. :contentReference[oaicite:1]{index=1}  
- Game Theory Explorer homepage: GTE website. :contentReference[oaicite:2]{index=2}

---

## Quick reproduction (Google Colab)

**Recommended runtime**
- Use the default Colab Python runtime (Colab keeps the runtime up-to-date; recent runtimes use Python 3.10–3.11). See Colab runtime docs for details. 

**Install required packages (first code cell)**  
Run this at the top of the notebook to install and import everything needed:
```python
!pip install -q nashpy quantecon numpy matplotlib
import numpy as np
import nashpy as nash
import quantecon.game_theory as gt
import matplotlib.pyplot as plt
