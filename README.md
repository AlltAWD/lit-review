# Literature Review — Learning-Based Visuomotor Manipulation

Twelve papers on getting learned manipulation policies to work on real, imperfect hardware,
read as background for my sim-to-real work on a low-cost SO-101 arm
([so-101-arm](https://github.com/AlltAWD/so-101-arm)). Three threads:

1. **Imitation learning for manipulation** — ACT, Diffusion Policy, and successors
2. **Sim-to-real transfer** — domain randomization and successors
3. **Visuomotor policies** — camera-in-the-loop control, up to vision-language-action models

Each note is one paragraph — **the problem, the method, the result** — with the verified title,
authors and a link to the paper. All 12 notes were written September–October 2026.

## Index

### Batch 1 — foundations

- [Tobin 2017](papers/tobin2017-domain-randomization.md) — Training only on domain-randomized rendered images skips real-world image collection and still gives an accurate, robust real-world detector.
- [Zhao 2023 (ACT)](papers/zhao2023-act.md) — Predicting chunks of future joint positions lets a low-cost leader-follower arm learn fine bimanual tasks at 80–90% success from just 50 demonstrations.
- [Chi 2023 (Diffusion Policy)](papers/chi2023-diffusion-policy.md) — Generating action sequences by iterative denoising handles multimodal demonstrations and beats prior methods by 46.9% on average across 15 tasks.

### Batch 2 — imitation learning for manipulation

- [Mandlekar 2021 (robomimic)](papers/mandlekar2021-robomimic.md) — Observation history, camera choice, and image augmentation matter when learning from human demonstrations.
- [Florence 2021 (Implicit BC)](papers/florence2021-implicit-bc.md) — Searching a learned energy function handles multiple valid actions and abrupt changes in behavior.
- [Fu 2024 (Mobile ALOHA)](papers/fu2024-mobile-aloha.md) — Co-training with static ALOHA data improves mobile manipulation with few target-task demonstrations.

### Batch 3 — sim-to-real for control

- [Peng 2018 (dynamics randomization)](papers/peng2018-dynamics-randomization.md) — Randomizing simulation dynamics lets a recurrent control policy transfer directly to a real robot.
- [OpenAI 2019 (Rubik's Cube / ADR)](papers/openai2019-rubiks-cube.md) — Automatically adjusting randomization ranges enables sim-to-real transfer for dexterous cube manipulation.
- [James 2019 (RCAN)](papers/james2019-sim-to-sim.md) — Translating images into a canonical simulation appearance enables grasping transfer without real training data.

### Batch 4 — the map, then where the field is now

- [Zhao 2020 (sim-to-real survey)](papers/zhao2020-sim-to-real-survey.md) — Maps the main sim-to-real approaches and their applications.
- [Brohan 2022 (RT-1)](papers/brohan2022-rt1.md) — A language-conditioned Transformer trained on diverse demonstrations generalizes to new combinations of skills and objects.
- [Shukor 2025 (SmolVLA)](papers/shukor2025-smolvla.md) — A compact vision-language-action model learns from community data and outperforms ACT on the studied SO-101 task.
