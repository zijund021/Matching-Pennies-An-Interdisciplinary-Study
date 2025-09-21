# Part 1 — Economist (theory & welfare)
## 1. ⚖️Equilibrium concept
I adopt *Nash equilibrium in mixed strategies* as the appropriate concept for *Matching Pennies*.  
A normal-form (strategic) game is $G=(N,(S_i)_{i\in N},(u_i)_{i\in N})$: a finite player set $N$; each player $i$ has a pure-strategy set $S_i$; and a payoff function $u_i:\prod_{j\in N} S_j \to \mathbb{R}$ (Osborne 2003, 11).  
A mixed strategy $\sigma_i$ is a probability distribution over $S_i$ (Osborne 2003, 115–16).  
For a mixed profile $\sigma=(\sigma_1,\sigma_2)$, expected payoffs are defined in the standard way by taking expectations over pure profiles; existence of a mixed-strategy Nash equilibrium in any finite normal-form game follows from fixed-point arguments (Nash 1951, 286–295).

## 2. 🧐Analytical solution, efficiency, and fairness

**Characterization.** In *Matching Pennies*, $S_1=S_2=\{H,T\}$. The canonical payoff matrix is:

|       | H       | T       |
|------:|:-------:|:-------:|
| **H** | (1, -1) | (-1, 1) |
| **T** | (-1, 1) | (1, -1) |

Osborne’s *Example 17.1* lays out the game and its interpretation (Osborne 2003, 28). There is no pure-strategy Nash equilibrium: each pure profile gives one player a profitable deviation (Osborne 2003, 38). Let player 1 choose $H$ with probability $p$, player 2 with probability $q$. Indifference conditions yield $q=\tfrac12$ and, symmetrically, $p=\tfrac12$; thus the unique mixed-strategy equilibrium is $(p,q)=(\tfrac12,\tfrac12)$ (Osborne 2003, 119–120).

**Efficiency and fairness.** The game is zero-sum, so utilitarian welfare (the sum of expected payoffs) is always zero. Ex ante Pareto improvements are impossible because one player’s gain exactly equals the other’s loss. The equilibrium is symmetric, giving both players equal expected payoff (zero), which supports an equity interpretation ex ante.

## 3. ✏️Interpretation, refinements, and tractability

**Realism.** Perfect 50–50 randomization may be behaviorally demanding; subjects can display biases or patterns.

**Multiplicity and refinements.** *Matching Pennies* has a *unique* mixed-strategy equilibrium (no pure or additional mixed equilibria) (Osborne 2003, 119–120). Refinements (e.g., trembling-hand) or noisy best response models (e.g., quantal response) can rationalize systematic deviations from perfect mixing.

**Computational tractability.** For a $2\times2$ game, the equilibrium is analytically immediate; larger games may require algorithms, even though existence is guaranteed by Nash’s theorem (Nash 1951, 286–295).



### 🧑‍🔬References 
- Baye, Michael R., Dan Kovenock, and Casper G. de Vries. 1996. “The All-Pay Auction with Complete Information.” Economic Theory 8 (2): 291–305. \url{https://doi.org/10.1007/BF01211819}
- Camerer, Colin F. 2003. *Behavioral Game Theory: Experiments in Strategic Interaction*. Princeton, NJ: Princeton University Press.
- Chen, Daniel L., Martin Schonger, and Chris Wickens. 2016. “oTree—An Open-Source Platform for Laboratory, Online, and Field Experiments.” *Journal of Behavioral and Experimental Finance* 9: 88–97. https://doi.org/10.1016/j.jbef.2015.12.001.
- Kagel, John H., and Dan Levin. 1986. “The Winner’s Curse and Public Information in Common Value Auctions.” American Economic Review 76 (5): 894–920.
- Knight, Vincent. 2021. *Nashpy: A Python Library for the Computation of Equilibria of 2-Player Strategic Games*, Version 0.0.28. Documentation. https://nashpy.readthedocs.io/en/v0.0.28/.
- Nash, John F. 1951. “Non-Cooperative Games.” *Annals of Mathematics* 54 (2): 286–295.
- Osborne, Martin J. 2003. *An Introduction to Game Theory*. New York: Oxford University Press.
- Savani, Rahul, and Bernhard von Stengel. 2015. “Game Theory Explorer—Software for the Applied Game Theorist.” *Computational Management Science* 12: 5–33.
- Sargent, Thomas J., and John Stachurski. 2021. *Quantitative Economics with Python*, Version 0.5.1. Online book. https://python.quantecon.org/.
