# SmolVLA: A Vision-Language-Action Model for Affordable and Efficient Robotics

**Authors / year:** Mustafa Shukor, Dana Aubakirova, Francesco Capuano, et al. / 2025
**Link:** https://arxiv.org/abs/2506.01844
**PDF:** [Local copy](<../../Zotero/storage/QR2Q75XC/Shukor et al. - 2025 - SmolVLA A Vision-Language-Action Model for Affordable and Efficient Robotics.pdf>)
**Zotero:** [Item](zotero://select/library/items/SBK5CABF) · [Read PDF](zotero://open-pdf/library/items/QR2Q75XC)
**Batch:** 4 — the map, then where the field is now (paper 12)
**Read on:** 10/28/2026

**Problem.** What were they unable to do before this paper?

Large vision-language-action models are expensive to train and deploy, limiting their usefulness on affordable robots and consumer hardware.

**Method.** In two or three sentences. What is the actual mechanism?

SmolVLA combines a frozen vision-language model with a flow-matching action expert that transforms noise into action chunks conditioned on images, instructions, and robot state. It learns from community demonstrations; asynchronous execution overlaps action prediction with robot movement.

**Result.** The number that matters, and on what task.

On SO-101 pick-and-place, the 450M-parameter model scored 90% versus ACT's 70% at familiar object positions, and 50% versus 40% at novel positions. These scores include partial credit for completed subtasks (Table 4).

**Why I care.**

A language-conditioned alternative to ACT, tested directly on my SO-101 platform and available through LeRobot.
