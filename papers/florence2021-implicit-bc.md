# Implicit Behavioral Cloning

**Authors / year:** Pete Florence, Corey Lynch, Andy Zeng, Oscar Ramirez, Ayzaan Wahid, Laura Downs, Adrian Wong, Johnny Lee, Igor Mordatch, Jonathan Tompson / 2021
**Link:** https://arxiv.org/abs/2109.00137
**PDF:** [Local copy](<../../Zotero/storage/PBI3MLSM/Florence et al. - 2021 - Implicit Behavioral Cloning.pdf>)
**Zotero:** [Item](zotero://select/library/items/IQIDVYLQ) · [Read PDF](zotero://open-pdf/library/items/PBI3MLSM)
**Batch:** 2 — imitation learning for manipulation (paper 5)
**Read on:** 10/27/2026

**Problem.** What were they unable to do before this paper?

Direct action prediction struggles with multiple valid actions and abrupt changes during contact. Mean squared error can average incompatible actions into an unsuccessful movement.

**Method.** In two or three sentences. What is the actual mechanism?

An energy-based model scores observation–action pairs, learning to assign demonstrated actions lower energy than sampled alternatives. At inference, it searches for a low-energy action instead of predicting one directly, allowing multiple valid actions and sharp changes in behavior.

**Result.** The number that matters, and on what task.

On real xArm6 block pushing with multiple valid targets and orders, implicit BC achieved 88.3% success versus 55.0% for explicit MSE-based BC, using 410 demonstrations and 60 evaluation trials per method (Table 6).

**Why I care.**

A baseline for SO-101 tasks with several valid solutions or precise contact, though action search adds computation.
