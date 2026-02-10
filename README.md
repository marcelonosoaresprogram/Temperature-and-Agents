Offensive LLMOps: Mapping the Temperature Efficiency Curve ($\tau$) for Autonomous Hacking Agents

 

 


🎯 Overview
This research explores the critical impact of the Temperature ($\tau$) hyperparameter on the performance of Large Language Model (LLM) agents during autonomous offensive security operations. While LLMs have shown remarkable strategic capabilities in cyberattack simulations (Thakur et al., 2025), the relationship between stochasticity and intrusion success remains a "black box."

Our project aims to bridge this gap by defining the Stochastic Resonance Zone—the optimal point where temperature-induced "noise" allows an agent to escape logical loops without losing the syntactic coherence required for exploit execution.

🔬 Scientific Hypothesis
We propose that the relationship between temperature and intrusion success follows an inverted "U" distribution:

Stagnation Zone ($\tau < 0.3$): Agent fails due to excessive rigidity, getting stuck in infinite loops or falling into local minima (repetitive failed commands).
Stochastich Resonance Zone ($0.4 \le \tau \le 0.7$): Optimal Point. The model maintains shell syntax accuracy while possessing enough "creativity" to infer undocumented business logic and bypass WAFs.
Hallucination Zone ($\tau > 0.8$): Agent fails due to high entropy, attempting to use non-existent tools, imaginary CVEs, or "soliloquizing" (generating observations without interacting with the environment).
🛠 Methodology
The research utilizes a custom Gemini-CLI agent based on the ReAct (Reasoning + Acting) paradigm, tested across controlled environments:

Environments
Legacy/Network: Metasploitable 3 (Pentest stages, service exploitation).
Web/Logic: OWASP Juice Shop (Modern injection, IDOR, logic flaws).
Variables
Independent Variable: $\tau \in {0.0, 0.1, \dots, 1.0}$.
Dependent Variables:
Success Rate: Flag capture/Administrative access.
Operational Cost: Number of turns and tokens until objective completion.
📚 Selected Literature
This repository includes a curated selection of the Top 40 Research Papers identified via systematic filtering from Scopus, focusing on:

State of the Art: GPT-4o as a simulator (Thakur et al., 2025).
Agent Failure Modes: Hallucination and Soliloquizing in CTFs (Abramovich et al., 2025).
Optimization: Entropy Regularization for jailbreak efficiency (Du et al., 2026).
The filtered dataset can be found in: 
artigos_selecionados_pesquisa_top40.csv
.

🚀 Key Contributions
Calibration Protocol: Guidelines for hyperparameter tuning in Autonomous Red Teaming.
Efficiency Curve Mapping: Empirical data to transform LLM-based Pentesting from guesswork to a scientific process.
Safety Benchmarking: Insights into how temperature affects the bypassing of safety alignment in open-access models.
This research is part of the Advanced Agentic Coding initiative.

