# Diffusion Policy: Visuomotor Policy Learning via Action Diffusion

**Authors / year:** Cheng Chi, Zhenjia Xu, Siyuan Feng, Eric Cousineau, Yilun Du, Benjamin Burchfiel, Russ Tedrake, Shuran Song 2023
**Link:** https://arxiv.org/abs/2303.04137
**Read on:** 10/01/2026

**Problem.** What were they unable to do before this paper?

Existing robot learning policies struggle with multimodal action distributions (several valid ways to do a task) and high-dimensional action spaces, and energy-based policies like Implicit BC are unstable to train.

**Method.** In two or three sentences. What is the actual mechanism?

The policy is a conditional denoising diffusion process: it starts from random noise and iteratively denoises it into a sequence of future actions, conditioned on the camera observations. It learns the gradient of the action-distribution score function and follows it at inference through a series of stochastic Langevin dynamics steps.

**Result.** The number that matters, and on what task.

Outperformed existing state-of-the-art methods by 46.9% on average across 15 tasks from 4 robot manipulation benchmarks.

**Why I care.**

A strong policy choice for the SO-101 on tasks that need smooth action sequences or have several valid ways to succeed.