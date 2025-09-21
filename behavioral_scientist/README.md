# Behavioral Scientist (oTree + LLM)

This folder contains the oTree app, screenshots, and LLM session artifacts for behavioral experiments.

---

## Deployment Steps

To run the oTree app locally:

1. Download `Matching_Pennies.otreezip` from this folder.  
2. Install Visual Studio Code (optional, for editing).  
3. Open a terminal / command prompt in the folder containing `Matching_Pennies.otreezip`.  
4. Install oTree:
   ```bash
   pip3 install -U otree
   otree zipserver
In browser, visit the local link shown (e.g. http://localhost:8000) to play the game.


## LLM Session Artifacts

The llm/ folder includes:

prompt#1&2.txt — exact prompts given to the LLM in both conditions

transcript#1.md transcript#2.md— full log of choices and reasoning from the LLM for each round

settings#1.json settings#2.json— the configuration used (model name, temperature, visibility condition, random seed, etc.)


## Session Config

Number of rounds: 7

Payment rule: One randomly selected round is used for payment (so every round is incentive-relevant)

Roles:

Player 1 = Mismatcher (wins if choices mismatch)

Player 2 = Matcher (wins if choices match)

Opponent type: human in all rounds

Visibility conditions: LLM session uses two conditions:

Rule-only (no payoff matrix shown)

Full-matrix (payoff matrix shown)


## Screenshots

Screenshots of game pages & session results are in screenshots/. You will find:

instructions pages

decision screens per round

final results and payoffs


## Ethics Note

No deception: participants are informed of all rules (including payment rule, payoff condition).

Informed consent: players know that one random round will be used for real payment.

Privacy: transcripts/screen captures do not include personal identifying information.

Equal treatment: both players have same information under same prompt conditions; changes in prompt only affect visibility, not fairness of rules.


## 🐱References 
- Baye, Michael R., Dan Kovenock, and Casper G. de Vries. 1996. “The All-Pay Auction with Complete Information.” Economic Theory 8 (2): 291–305. \url{https://doi.org/10.1007/BF01211819}
- Camerer, Colin F. 2003. *Behavioral Game Theory: Experiments in Strategic Interaction*. Princeton, NJ: Princeton University Press.
- Chen, Daniel L., Martin Schonger, and Chris Wickens. 2016. “oTree—An Open-Source Platform for Laboratory, Online, and Field Experiments.” *Journal of Behavioral and Experimental Finance* 9: 88–97. https://doi.org/10.1016/j.jbef.2015.12.001.
- Kagel, John H., and Dan Levin. 1986. “The Winner’s Curse and Public Information in Common Value Auctions.” American Economic Review 76 (5): 894–920.
- Knight, Vincent. 2021. *Nashpy: A Python Library for the Computation of Equilibria of 2-Player Strategic Games*, Version 0.0.28. Documentation. https://nashpy.readthedocs.io/en/v0.0.28/.
- Nash, John F. 1951. “Non-Cooperative Games.” *Annals of Mathematics* 54 (2): 286–295.
- Osborne, Martin J. 2003. *An Introduction to Game Theory*. New York: Oxford University Press.
- Savani, Rahul, and Bernhard von Stengel. 2015. “Game Theory Explorer—Software for the Applied Game Theorist.” *Computational Management Science* 12: 5–33.
- Sargent, Thomas J., and John Stachurski. 2021. *Quantitative Economics with Python*, Version 0.5.1. Online book. https://python.quantecon.org/.
