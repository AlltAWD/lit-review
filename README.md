# Literature Review — Learning-Based Visuomotor Manipulation

Scope: **12 papers in four batches of three.** Three threads only:

1. **Imitation learning for manipulation** — ACT, Diffusion Policy
2. **Sim-to-real transfer** — domain randomization and successors
3. **Visuomotor policies** — camera-in-the-loop control

Purpose: (a) the written half of the Eliott audition, (b) reusable material for
REU applications and the 3-2 statement of purpose.

One paragraph per paper: **what problem, what method, what result.** That is the
whole format. Do not write more; do not read the full paper on the first pass.

## Progress

| Batch | Papers | Focus | Notes written |
|---|---|---|---|
| 1 | 1–3 | Foundations | 3/3 |
| 2 | 4–6 | Imitation learning for manipulation | 3/3 |
| 3 | 7–9 | Sim-to-real for control | 3/3 |
| 4 | 10–12 | Survey, RT-1, SmolVLA | 3/3 |

Batches 2–4 have notes with verified titles, authors, paper links, and
local PDF/Zotero links. All 12 notes are filled in and dated.
The PDFs are attached to their records in Zotero under
**Robotics & Engineering → Literature Review**, tagged `lit-review-batch-2`,
`lit-review-batch-3`, or `lit-review-batch-4`.

Allow about 20 minutes per paper: abstract, figure 1 and the method figure,
contributions, conclusion/limitations, then write from memory and check one number.
For the Rubik's Cube paper, read only the abstract and ADR section; for the survey,
use the section headings as a map for the later synthesis.

## Index

### Batch 1 — foundations

Completed notes:

- [Tobin 2017](papers/tobin2017-domain-randomization.md) — Training only on domain-randomized rendered images skips real-world image collection and still gives an accurate, robust real-world detector.
- [Zhao 2023 (ACT)](papers/zhao2023-act.md) — Predicting chunks of future joint positions lets a low-cost leader-follower arm learn fine bimanual tasks at 80–90% success from just 50 demonstrations.
- [Chi 2023 (Diffusion Policy)](papers/chi2023-diffusion-policy.md) — Generating action sequences by iterative denoising handles multimodal demonstrations and beats prior methods by 46.9% on average across 15 tasks.

### Batch 2 — imitation learning for manipulation

- [x] [Mandlekar 2021 (robomimic)](papers/mandlekar2021-robomimic.md) — Observation history, camera choice, and image augmentation matter when learning from human demonstrations.
- [x] [Florence 2021 (Implicit BC)](papers/florence2021-implicit-bc.md) — Searching a learned energy function handles multiple valid actions and abrupt changes in behavior.
- [x] [Fu 2024 (Mobile ALOHA)](papers/fu2024-mobile-aloha.md) — Co-training with static ALOHA data improves mobile manipulation with few target-task demonstrations.

### Batch 3 — sim-to-real for control

- [x] [Peng 2018 (dynamics randomization)](papers/peng2018-dynamics-randomization.md) — Randomizing simulation dynamics lets a recurrent control policy transfer directly to a real robot.
- [x] [OpenAI 2019 (Rubik's Cube / ADR)](papers/openai2019-rubiks-cube.md) — Automatically adjusting randomization ranges enables sim-to-real transfer for dexterous cube manipulation.
- [x] [James 2019 (RCAN)](papers/james2019-sim-to-sim.md) — Translating images into a canonical simulation appearance enables grasping transfer without real training data.

### Batch 4 — the map, then where the field is now

- [x] [Zhao 2020 (sim-to-real survey)](papers/zhao2020-sim-to-real-survey.md) — Maps the main sim-to-real approaches and their applications, providing a structure for the synthesis.
- [x] [Brohan 2022 (RT-1)](papers/brohan2022-rt1.md) — A language-conditioned Transformer trained on diverse demonstrations generalizes to new combinations of skills and objects.
- [x] [Shukor 2025 (SmolVLA)](papers/shukor2025-smolvla.md) — A compact vision-language-action model learns from community data and outperforms ACT on the studied SO-101 task.
