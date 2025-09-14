# Computational Scientist (normal form + GTE)

This folder contains the Colab notebook and GTE exports used to compute and visualize the mixed Nash equilibrium for Matching Pennies.

## Contents
- `notebook.ipynb` — Colab-exported Jupyter notebook.  
- `README.md` — this file (how-to-run and notes).  
- `GTE.png` — (optional) GTE export images/graphics.  

---

## Quick reproduction (Google Colab)

**Recommended runtime**
- Use the default Colab Python runtime (Colab keeps the runtime up-to-date; recent runtimes use Python 3.10–3.11). See Colab runtime docs for details. 

**Install required packages (first code cell)**  
Run this at the top of the notebook to install and import everything needed:

```python
# Colab setup cell — run once at the start
!pip install -q nashpy quantecon numpy matplotlib

# imports
import numpy as np
import nashpy as nash
import quantecon.game_theory as gt
import matplotlib.pyplot as plt

# reproducibility: set numpy/random seeds
SEED = 20250914
np.random.seed(SEED)

# Matching Pennies payoff matrices (row = Player 1, col = Player 2)
A = np.array([[ 1, -1],
              [-1,  1]])   # Row player
B = -A                    # Column player (zero-sum)

# NashPy: construct and solve
game = nash.Game(A, B)
print("Game object:")
print(game)

# support enumeration (mixed NE)
equilibria = list(game.support_enumeration())
print("NashPy support_enumeration results:", equilibria)

# QuantEcon alternative (NormalFormGame)
mp_matrix = np.array([[( 1, -1), (-1,  1)],
                      [(-1,  1), ( 1, -1)]])
g_mp = gt.NormalFormGame(mp_matrix)
print("QuantEcon NormalFormGame summary:")
print(g_mp)

# QuantEcon solvers
print("QuantEcon pure_nash_brute:", gt.pure_nash_brute(g_mp))
print("QuantEcon support_enumeration:", gt.support_enumeration(g_mp))
print("QuantEcon vertex_enumeration:", gt.vertex_enumeration(g_mp))


## GTE (Game Theory Explorer) — extensive-form illustration & exports

This directory holds GTE exports: extensive-form tree, strategic-form matrix, and solver output for Matching Pennies.

