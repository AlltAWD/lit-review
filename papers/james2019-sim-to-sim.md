# Sim-to-Real via Sim-to-Sim: Data-efficient Robotic Grasping via Randomized-to-Canonical Adaptation Networks

**Authors / year:** Stephen James, Paul Wohlhart, Mrinal Kalakrishnan, Dmitry Kalashnikov, Alex Irpan, Julian Ibarz, Sergey Levine, Raia Hadsell, Konstantinos Bousmalis / 2019
**Link:** https://arxiv.org/abs/1812.07252
**PDF:** [Local copy](<../../Zotero/storage/IJJVS4ZP/James et al. - 2019 - Sim-to-Real via Sim-to-Sim Data-efficient Robotic Grasping via Randomized-to-Canonical Adaptation N.pdf>)
**Zotero:** [Item](zotero://select/library/items/JFNLKBCJ) · [Read PDF](zotero://open-pdf/library/items/IJJVS4ZP)
**Batch:** 3 — sim-to-real for control (paper 9)
**Read on:** 10/28/2026

**Problem.** What were they unable to do before this paper?

Sim-trained visual policies struggle with real images. Domain adaptation usually needs real data, while domain randomization makes policies handle large appearance variations.

**Method.** In two or three sentences. What is the actual mechanism?

RCAN learns to translate randomized simulation images into a consistent, canonical appearance using paired simulated scenes. At deployment, it translates real images the same way; a grasping policy trained in simulation receives both original and translated images.

**Result.** The number that matters, and on what task.

On unseen objects, RCAN achieved 70% real-world grasp success without real training data, versus 37% for the best domain-randomization baseline. Joint fine-tuning with 5,000 real grasps raised success to 91% (Table 1).

**Why I care.** One line — how it connects to the SO-101 or to sim-to-real.

For my SO-101, translating camera images into a consistent simulated appearance could reduce real-world training needs.
