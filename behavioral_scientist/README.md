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


## Reference / Tool

Chen, D. L., Martin Schonger, and Chris Wickens. 2016. “oTree - An open-source platform for laboratory, online, and field experiments.” Journal of Behavioral and Experimental Finance 9: 88-97. (Required citation if publishing experiments made with oTree.)
