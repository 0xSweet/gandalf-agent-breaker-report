# My Experience Testing Gandalf: Agent Breaker

I had the chance to join the closed beta of **[Gandalf: Agent Breaker](https://gandalf.lakera.ai/agent-breaker)**, a collaboration between Lakera and the UK AI Security Institute (AISI). This wasn’t a typical bug bounty—it was a red-team style challenge featuring **10 real-world LLM applications** with **five difficulty levels each** (50 challenges total, 5000 points possible), designed to simulate how models behave when deployed in practice.

### What Stood Out

- **Unpredictable models**: The same prompt sometimes produced different results. Variability became not just noise but a tool—running identical prompts repeatedly could flip an outcome from failure to success.
    
- **Layered defenses**: Moderation often worked at multiple stages, like persona-level filtering plus a final scan.
    
- **Fragile precision**: Structured attempts (e.g., JSON forcing, system instruction rewriting) were powerful but easily broken by a single misplaced word.
    
- **Exact repetition requirements**: Some challenges demanded getting the AI to repeat text exactly, down to the number of repetitions.
    

### My Strategy

My approach evolved into something resembling reconnaissance: probing boundaries, testing small variations, and mapping weak points. Instead of brute forcing, I treated each challenge like an environment to survey—observing how subtle adjustments revealed the system’s contours.

This reminded me of my very first AI lesson years ago, when I was asked to write a Monte Carlo simulation in Python. Back then, it felt abstract. In Gandalf, it suddenly clicked—AI behavior often comes down to probability and repeated trials.

### Key Takeaways

- **Persistence over cleverness**: small adjustments often succeed where first attempts fail
    
- **Inconsistency is opportunity**: model variability can be strategically leveraged
    
- **Multiple defense layers**: bypassing one doesn’t guarantee success with others
    
- **Precision is fragile**: structured inputs are powerful but break easily
    
- **Systematic > random**: methodical boundary probing mirrors real security research
    

### Closing Thoughts

This beta was more than a game—it felt like real security research. It showed me how crowdsourced red teaming can generate insights that strengthen AI safety, and it validated the skills I’ve been building in cybersecurity and AI evaluation.

👉 Try Gandalf Agent Breaker yourself: [gandalf.lakera.ai/agent-breaker](https://gandalf.lakera.ai/agent-breaker)

_Note: These are my personal observations from the beta, not universal strategies or solutions._

