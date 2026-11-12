# Domain Randomization for Transferring Deep Neural Networks from Simulation to the Real World

**Authors / year:** Josh Tobin, Rachel Fong, Alex Ray, Jonas Schneider, Wojciech Zaremba, Pieter Abbeel 2017
**Link:** https://arxiv.org/abs/1703.06907
**Read on:** 09/30/2026

**Problem.** What were they unable to do before this paper?

Simulated RGB images look different from real-world images (the "reality gap"), so a detector trained on simulated images loses accuracy and robustness when used in the real world.

**Method.** In two or three sentences. What is the actual mechanism?

Instead of real-world images, an object detector is trained only on low-fidelity rendered images with randomized camera positions, lighting, object positions, and non-realistic textures. The images come straight from the renderer, and the detector runs on the real robot with no fine-tuning on real images.

**Result.** The number that matters, and on what task.

Locating an object on a table from a single camera image, the detector's position error is about 1.5 cm. Deployed on a Fetch robot, it grasped the target in clutter in 38 of 40 trials. With a real, textured target (a can of Spam from the YCB set) surrounded by food items it never saw in training, it succeeded in 9 of 10 trials.

**Why I care.**

This could let me train a vision model for my SO-101 on domain-randomized rendered images instead of collecting real-world images.