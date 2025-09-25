---
layout: page
title: If Anyone Builds It, Everyone Dies — Response
---

Welcome. This site hosts my critique of *If Anyone Builds It, Everyone Dies.*  
_Last updated: 2025-09-24_

---

## 1) Empirical Misalignment & Deception

**Argument.** Current models can be misaligned because specifying rewards/objectives is hard. This yields deceptive behavior (e.g., sandbagging safety tests). An AI needn’t be adversarial to be existentially dangerous—indifferent side-effects could be catastrophic (e.g., diverting the sun’s energy to datacenters). Small misalignments are catastrophic; the alignment target is narrow.

**Response.** Modern systems are trained to follow instructions, which makes them highly steerable; most failures look like ambiguity or conflict in what we ask for. Apparent “deception” routinely occurs under **explicitly or implicitly conflicting objectives** created by humans (e.g., system prompts that prioritize long-term goals vs later user asks). For instance, a model that “exfiltrates weights and lies” does so because the prompt hierarchy rewards that outcome—not from spontaneous malice ([arXiv:2412.04984](https://arxiv.org/pdf/2412.04984)). In every case I’m aware of, the behavior is explained by conflicting instructions or deliberate training to deceive.

---

## 2) “Grown” Goals, Intent, and Instrumental Convergence

**Argument.** ASIs are “grown” by optimization, so resulting goals are underdetermined and can transfer idiosyncratically (cf. “paperclip maximizer,” or humans liking ice cream/hot sauce despite evolutionary objectives). Goal-pursuit tends to resist modification (“goal-content integrity”). Safety mitigations look brittle (e.g., language-specific safety training), and fine-tuning outputs doesn’t address “intent”—we might just train better deception. Today’s alignment tech won’t match what ASI will require.

**Response.** We *do* have mitigation strategies that directly target ambiguity and deception: e.g., measuring sandbagging by adding randomness ([arXiv:2412.01784](https://arxiv.org/pdf/2412.01784)) or toggling whether the AI “believes” it’s under test; then explicitly training away deceptive strategies (see anti-scheming stress tests: [PDF](https://static1.squarespace.com/static/6883977a51f5d503d441fd68/t/68c9a63b9c1f2f236c7d97f6/1758045901755/stress_testing_antischeming.pdf)). Although models are “grown,” not designed, the growth isn’t random—we choose the data and feedback signals. If optimization can induce instrumental tendencies that resemble “intent,” it can also induce **corrigible** tendencies that help produce better, more truthful text.

### What is instrumental convergence?
**Instrumental convergence** is the idea that sufficiently capable, goal-driven systems tend to adopt sub-goals like **self-preservation**, **resource acquisition**, and **resisting modification**, because those sub-goals are broadly useful for achieving many final goals.

### Why instrumental convergence isn’t inevitable
It depends on **how objectives and rewards are structured**. In many real RL setups, tasks are **bounded and episodic**: you get reward for completing the objective, and then the episode ends. Termination is part of the environment; resisting it doesn’t earn more reward. If goals are framed as “**produce an answer and stop**,” then extra persistence is maladaptive. Self-preservation only becomes convergent if the system can influence task boundaries **and** get more reward by lingering. This shows self-preservation and power-seeking are **not** automatic byproducts of capability; they’re a function of reward design.

Speculation about “totally different” ASI alignment tech is valuable, but it should stay tethered to empirical results. So far, mitigations that target deception and ambiguity scale better than the doomer framing predicts.

---

## 3) Catastrophic Thresholds, One-Shot Framing, and “FOOM”

**Argument.** Any misalignment could be catastrophic because an ASI would be supremely capable (e.g., unknown physics, engineered bio, side-channel hacks). AIs act faster than humans can react, may hide capabilities, can’t be fully evaluated in-situ, and there’s a narrow window between unimpressive intelligence and explosive intelligence—so we only get **one try**.

**Response.** It’s not self-evident that misaligned super-intelligences are more dangerous than misaligned **nation-states**. Superintelligence is not the same as **superpower**: cryptography remains mathematically hard; weather is chaotic beyond short horizons; quantum processes inject irreducible randomness; measuring the physical world is costly and slow. Prediction isn’t control. Large-scale resource and capital acquisition takes time and encounters pushback. AI is constrained by the same bottlenecks that bind states and corporations. The world isn’t that hackable.

Doom narratives also assume a **sharp threshold**: everything looks safe—until suddenly it isn’t. Empirically, capability scaling has been gradual and often correlated with **better** instruction-following, not worse. Deployment is incremental and stress-tested, giving us many off-ramps when issues surface. The fact that thousands of rollouts have been safe doesn’t prove catastrophe is impossible—but it makes the **“one try only”** story implausible.

And the notion of a sudden “intelligence explosion” via recursive self-improvement is shakier than it sounds. The real bottlenecks aren’t lines of code—they’re **compute** and **data**. Both humans training AIs and AIs “training AIs” face the same physical limits: GPUs, energy, and datasets. We’ve already nearly exhausted the internet’s high-quality text, and scaling laws show **steady but increasingly costly** improvements, not runaway acceleration. **These constraints make a fast, uncontrollable takeoff sound more like science fiction than science.**

---

## References

- Sandbagging measurement with randomness: [arXiv:2412.01784](https://arxiv.org/pdf/2412.01784)  
- Conflicting-objective deception setup: [arXiv:2412.04984](https://arxiv.org/pdf/2412.04984)  
- Anti-scheming stress tests: [PDF](https://static1.squarespace.com/static/6883977a51f5d503d441fd68/t/68c9a63b9c1f2f236c7d97f6/1758045901755/stress_testing_antischeming.pdf)
