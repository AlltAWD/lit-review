# Literature Review — Learning-Based Visuomotor Manipulation

Scope cap: **~15 papers, not 50.** Three threads only:

1. **Imitation learning for manipulation** — ACT, Diffusion Policy
2. **Sim-to-real transfer** — domain randomization and successors
3. **Visuomotor policies** — camera-in-the-loop control

Purpose: (a) the written half of the Eliott audition, (b) reusable material for
REU applications and the 3-2 statement of purpose.

One paragraph per paper: **what problem, what method, what result.** That is the
whole format. Do not write more; do not read the full paper on the first pass.

## Progress

| Week | Target | Done |
|---|---|---|
| Sept 8–14 | 5 papers | |
| Sept 15–21 | 10 papers | |
| Sept 22–28 | 15 papers + synthesis started | |

## Index

_(add a line per paper as you go: `- [Short name](papers/short-name.md) — one-line takeaway`)_
- [Tobin 2017](papers/tobin2017-domain-randomization.md) — Training only on domain-randomized rendered images skips real-world image collection and still gives an accurate, robust real-world detector.
- [Zhao 2023 (ACT)](papers/zhao2023-act.md) — Predicting chunks of future joint positions lets a low-cost leader-follower arm learn fine bimanual tasks at 80–90% success from just 50 demonstrations.
- [Chi 2023 (Diffusion Policy)](papers/chi2023-diffusion-policy.md) — Generating action sequences by iterative denoising handles multimodal demonstrations and beats prior methods by 46.9% on average across 15 tasks.
