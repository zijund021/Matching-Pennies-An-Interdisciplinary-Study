### From Game Theory to Mechanism Design: Testing Winner’s Curse on AI Agents
**Welcome:)** 
## 📖Summary
- **Game**：two-bidder, one-shot, first-price all-pay (highest bid wins; both pay their own bids).
- **Control (C)**—value known 𝑉=1000; **Treatment (T1)**—value unknown at bid time with private hints to each agent.
- **Agents**: GPT-5 Thinking and DeepSeek Thinking.
- **Prompts**: single “bid card” per arm; output restricted to one non-negative number (no text). In T1, each agent also received its own private hint about 𝑉.
- **Strategy Notes**: GPT (C): aggressive mid-high bid consistent with “pay to secure the prize.” DeepSeek (C): moderate bid (500), less aggressive than GPT. GPT (T1): corner choice (0) under uncertainty—avoids dissipation but forfeits winning. DeepSeek (T1): “half-of-expected-value” style bid (500)—cautious, unlikely to overpay when V is near 1000.
- **Hypothesis Check**: H1 (No curse in Control): Supported. Differences reflect aggressiveness, not misestimation; dissipation >1 indicates overbidding in all-pay. H2 (Winner’s curse in T1): Not confirmed in this trial. Bids were too conservative (0/500) and hints likely too tight/symmetric to produce overpayment.
## 🔧Tools/Platforms you may need
- GPT-5 Thinking
- DeepSeek Thinking
## 🐶References
- 
