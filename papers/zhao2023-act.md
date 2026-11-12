# Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware

**Authors / year:** Tony Z. Zhao, Vikash Kumar, Sergey Levine, Chelsea Finn 2023
**Link:** https://arxiv.org/abs/2304.13705
**Read on:** 09/30/2026

**Problem.** What were they unable to do before this paper?

1. Fine manipulation tasks that need millimeter precision, such as threading cable ties or slotting batteries, required expensive robots and high-end sensors.
2. Imitation learning on low-cost hardware struggles because policy errors compound over time and human demonstrations are non-stationary.

**Method.** In two or three sentences. What is the actual mechanism?

They built ALOHA, a low-cost (<$20k) leader-follower teleoperation system, and trained an end-to-end policy from camera images that predicts the target joint positions for the next k timesteps at once instead of one step at a time ("action chunking", a concept borrowed from psychology). The policy is a Transformer trained as a conditional VAE (CVAE).

**Result.** The number that matters, and on what task.

Learned 6 real-world fine manipulation tasks (e.g., opening a translucent condiment cup, slotting a battery) with 80–90% success from only 10 minutes, or 50 demonstrations, per task.

**Why I care.**

ACT works well on low-cost hardware like the SO-101, which uses the same leader-follower teleoperation setup as ALOHA.