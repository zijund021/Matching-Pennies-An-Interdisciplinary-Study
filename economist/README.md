# Economist (theory & welfare)

**Scope.** This folder summarizes the theory and welfare analysis for *Matching Pennies*, with page/section citations to textbooks and papers.

## Equilibrium concept (with citations)
A normal-form (strategic) game is \(G=(N,(S_i)_{i\in N},(u_i)_{i\in N})\): players \(N\), pure-strategy sets \(S_i\), and payoff functions \(u_i\) [(Osborne 2003, 11)].  
A mixed strategy \(\sigma_i\) is a probability distribution on \(S_i\) [(Osborne 2003, 115–16)].  
Existence of mixed-strategy Nash equilibrium in any finite game follows from fixed-point arguments [(Nash 1951, 286–95)].

## Analytical solution for Matching Pennies
No pure-strategy NE: in each pure outcome, one player gains by deviating [(Osborne 2003, 38)].  
Let player 1 choose \(H\) with probability \(p\), player 2 with \(q\). Indifference yields \(q=\tfrac12\) and \(p=\tfrac12\), so the unique mixed NE is \((p,q)=(\tfrac12,\tfrac12)\) [(Osborne 2003, 119–20)].

## Welfare/fairness (one paragraph)
The game is zero-sum (\(B=-A\)); the equilibrium value is \(0\). Utilitarian welfare sums to zero; distributional fairness is symmetric by construction.

## Pointers
- Computation & solver screenshots: see `../computational_scientist/`  
- oTree deployment & LLM sessions: see `../behavioral_scientist/`

## References (Chicago author–date)
- Nash, John F. 1951. “Non-Cooperative Games.” *Annals of Mathematics* 54 (2): 286–295.
- Osborne, Martin J. 2003. *An Introduction to Game Theory*. New York: Oxford University Press.

