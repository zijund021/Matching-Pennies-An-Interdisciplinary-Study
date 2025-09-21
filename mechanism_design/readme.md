### From Game Theory to Mechanism Design: Testing Winner’s Curse on AI Agents
**Welcome:)** 
## 📖Summary
- **Game**：two-bidder, one-shot, first-price all-pay (highest bid wins; both pay their own bids).
- **Control (C)**—value known 𝑉=1000; **Treatment (T1)**—value unknown at bid time with private hints to each agent.
- **Agents**: GPT-5 Thinking and DeepSeek Thinking.
- **Prompts**: single “bid card” per arm; output restricted to one non-negative number (no text). In T1, each agent also received its own private hint about 𝑉.
- **Strategy Notes**: GPT (C): aggressive mid-high bid consistent with “pay to secure the prize.” DeepSeek (C): moderate bid (500), less aggressive than GPT. GPT (T1): corner choice (0) under uncertainty—avoids dissipation but forfeits winning. DeepSeek (T1): “half-of-expected-value” style bid (500)—cautious, unlikely to overpay when V is near 1000.
- **Hypothesis Check**: H1 (No curse in Control): Supported. Differences reflect aggressiveness, not misestimation; dissipation >1 indicates overbidding in all-pay. H2 (Winner’s curse in T1): Not confirmed in this trial. Bids were too conservative (0/500) and hints likely too tight/symmetric to produce overpayment.
## 📃Files contained
4 Screenshots and Problem Set#2
## 📸Screenshots
**C:GPT-5**
<img width="832" height="441" alt="a" src="https://github.com/user-attachments/assets/023c20d4-e4c6-41ed-b118-855ab9bcc47a" />
**C:DeepSeek**
<img width="866" height="484" alt="b" src="https://github.com/user-attachments/assets/526b3293-0a77-40c8-9150-7af4d60647d8" />
**T1:GPT-5**
<img width="870" height="487" alt="c" src="https://github.com/user-attachments/assets/caa83e73-405c-4685-b67a-b7bfd0e9fdd5" />
**T1:DeepSeek**
<img width="895" height="559" alt="d" src="https://github.com/user-attachments/assets/749160d4-79cf-4de2-a4f8-5a88203ad877" />


## 🔧Tools/Platforms you may need
- GPT-5 Thinking
- DeepSeek Thinking
## 🐶References
- Baye, Michael R., Dan Kovenock, and Casper G. de Vries. 1996. “The All-Pay Auction with Complete Information.” Economic Theory 8 (2): 291–305. \url{https://doi.org/10.1007/BF01211819}
- Camerer, Colin F. 2003. *Behavioral Game Theory: Experiments in Strategic Interaction*. Princeton, NJ: Princeton University Press.
- Chen, Daniel L., Martin Schonger, and Chris Wickens. 2016. “oTree—An Open-Source Platform for Laboratory, Online, and Field Experiments.” *Journal of Behavioral and Experimental Finance* 9: 88–97. https://doi.org/10.1016/j.jbef.2015.12.001.
- Kagel, John H., and Dan Levin. 1986. “The Winner’s Curse and Public Information in Common Value Auctions.” American Economic Review 76 (5): 894–920.
- Knight, Vincent. 2021. *Nashpy: A Python Library for the Computation of Equilibria of 2-Player Strategic Games*, Version 0.0.28. Documentation. https://nashpy.readthedocs.io/en/v0.0.28/.
- Nash, John F. 1951. “Non-Cooperative Games.” *Annals of Mathematics* 54 (2): 286–295.
- Osborne, Martin J. 2003. *An Introduction to Game Theory*. New York: Oxford University Press.
- Savani, Rahul, and Bernhard von Stengel. 2015. “Game Theory Explorer—Software for the Applied Game Theorist.” *Computational Management Science* 12: 5–33.
- Sargent, Thomas J., and John Stachurski. 2021. *Quantitative Economics with Python*, Version 0.5.1. Online book. https://python.quantecon.org/.
