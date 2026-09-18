# Frank Duah

I work on agent evaluation: measuring how reliably an LLM agent actually behaves, and catching it when it gets worse.

Normal software is deterministic, so a test gives you a verdict. Agents are not. The same prompt can pass nine times and fail the tenth, which means a single run tells you almost nothing. So you measure a rate instead, set it as a baseline, and fail the build when it drops.

MS in Artificial Intelligence at Northeastern (Khoury), with a background in software engineering and DevOps. I build things from first principles to understand them, then measure whether they hold up.

## What I'm building

**agentbounds** is an adversarial stress-tester for LLM agents. Point it at any agent, throw hostile and edge-case inputs at it, and get an honest report of where and how often it breaks. Zero runtime dependencies, 170 passing unit tests. Three decisions define it: hold rates over N trials instead of single verdicts, inconclusive judge calls excluded from the denominator instead of silently counted as passes, and heuristic detectors labelled as heuristic. The effect-assertion layer is still being built, and the README does not claim otherwise.

Alongside it, a set of from-scratch builds with no frameworks: [**Glassbox**](https://github.com/devfrankduah/glassbox), a transformer in NumPy with every gradient hand-derived and checked to 1e-8, covering both GPT-2 and Llama-style architectures. [**Forge**](https://github.com/devfrankduah/forge), LoRA, DoRA, and QLoRA-style int8 quantization implemented by hand with the frozen base provably untouched. **Cleave**, a byte-level BPE tokenizer with a provably lossless Unicode round-trip. **Winnow**, an MCP server written without an SDK that compacts documents and scans them for prompt injection.

## Open source

I'm a Collaborator and the second-highest contributor to [llm-exe](https://github.com/llm-exe/llm-exe), a provider-agnostic TypeScript framework for building LLM applications. I authored its multimodal text-and-image embedding input feature, merged upstream and shipped in v3.0.3. The work that got me there is mostly unglamorous: provider correctness, CI hardening, and the release pipeline.

[My 56 merged PRs](https://github.com/llm-exe/llm-exe/pulls?q=is%3Apr+author%3Adevfrankduah+is%3Amerged)

## Public repos

- [ML-Latency-Aware-Execution-Engine](https://github.com/devfrankduah/ML-Latency-Aware-Execution-Engine): reinforcement learning for crypto trade execution. A Double DQN with a dueling architecture and prioritized experience replay alongside classical models, validated against 98 million real market trades across 3 assets. Beats a TWAP baseline by 10.2 basis points on Bitcoin and cuts execution cost 96.7% versus immediate execution. 17 ablation studies, 176 unit tests.
- [music_mood_classification](https://github.com/devfrankduah/music_mood_classification): RoBERTa transfer learning predicting valence and arousal from lyrics. 0.781 valence and 0.649 arousal correlation on the MERGE Lyrics Complete split (2,568 lyrics).

Glassbox and Forge are public too, linked above. agentbounds, Cleave and Winnow are private while I finish cleaning them up. Write-ups for all of them are at [frankduah.me](https://www.frankduah.me).

## Elsewhere

[frankduah.me](https://www.frankduah.me) · [LinkedIn](https://www.linkedin.com/in/devfrankduah)
