# Part 1 — Economist (theory & welfare)
## 1. Equilibrium concept
I adopt *Nash equilibrium in mixed strategies* as the appropriate concept for *Matching Pennies*.  
A normal-form (strategic) game is $G=(N,(S_i)_{i\in N},(u_i)_{i\in N})$: a finite player set $N$; each player $i$ has a pure-strategy set $S_i$; and a payoff function $u_i:\prod_{j\in N} S_j \to \mathbb{R}$ (Osborne 2003, 11).  
A mixed strategy $\sigma_i$ is a probability distribution over $S_i$ (Osborne 2003, 115–16).  
For a mixed profile $\sigma=(\sigma_1,\sigma_2)$, expected payoffs are defined in the standard way by taking expectations over pure profiles; existence of a mixed-strategy Nash equilibrium in any finite normal-form game follows from fixed-point arguments (Nash 1951, 286–295).

## 2. Analytical solution, efficiency, and fairness

**Characterization.** In *Matching Pennies*, $S_1=S_2=\{H,T\}$. The canonical payoff matrix is:

|       | H       | T       |
|------:|:-------:|:-------:|
| **H** | (1, -1) | (-1, 1) |
| **T** | (-1, 1) | (1, -1) |

Osborne’s *Example 17.1* lays out the game and its interpretation (Osborne 2003, 28). There is no pure-strategy Nash equilibrium: each pure profile gives one player a profitable deviation (Osborne 2003, 38). Let player 1 choose $H$ with probability $p$, player 2 with probability $q$. Indifference conditions yield $q=\tfrac12$ and, symmetrically, $p=\tfrac12$; thus the unique mixed-strategy equilibrium is $(p,q)=(\tfrac12,\tfrac12)$ (Osborne 2003, 119–120).

**Efficiency and fairness.** The game is zero-sum, so utilitarian welfare (the sum of expected payoffs) is always zero. Ex ante Pareto improvements are impossible because one player’s gain exactly equals the other’s loss. The equilibrium is symmetric, giving both players equal expected payoff (zero), which supports an equity interpretation ex ante.

## 3. Interpretation, refinements, and tractability

**Realism.** Perfect 50–50 randomization may be behaviorally demanding; subjects can display biases or patterns.

**Multiplicity and refinements.** *Matching Pennies* has a *unique* mixed-strategy equilibrium (no pure or additional mixed equilibria) (Osborne 2003, 119–120). Refinements (e.g., trembling-hand) or noisy best response models (e.g., quantal response) can rationalize systematic deviations from perfect mixing.

**Computational tractability.** For a $2\times2$ game, the equilibrium is analytically immediate; larger games may require algorithms, even though existence is guaranteed by Nash’s theorem (Nash 1951, 286–295).
