# What Matters in Learning from Offline Human Demonstrations for Robot Manipulation

**Authors / year:** Ajay Mandlekar, Danfei Xu, Josiah Wong, Soroush Nasiriany, Chen Wang, Rohun Kulkarni, Li Fei-Fei, Silvio Savarese, Yuke Zhu, Roberto Martín-Martín / 2021
**Link:** https://arxiv.org/abs/2108.03298
**PDF:** [Local copy](<../../Zotero/storage/SPNANN5U/Mandlekar et al. - 2021 - What Matters in Learning from Offline Human Demonstrations for Robot Manipulation.pdf>)
**Zotero:** [Item](zotero://select/library/items/T4YE8Z9L) · [Read PDF](zotero://open-pdf/library/items/SPNANN5U)
**Batch:** 2 — imitation learning for manipulation (paper 4)
**Read on:** 10/27/2026

**Problem.** What were they unable to do before this paper?

Without shared human-demonstration datasets and reproducible benchmarks, it was difficult to compare offline learning methods for robot manipulation.

**Method.** In two or three sentences. What is the actual mechanism?

They released robomimic datasets and code, comparing six algorithms across five simulated and three real-world tasks. They varied data quality, dataset size, observations, and hyperparameters; recurrent behavioral cloning (BC-RNN), which remembers observation history, was a strong baseline.

**Result.** The number that matters, and on what task.

On real-world can pick-and-place, BC-RNN achieved 73.3% success over 30 trials using 200 demonstrations. Removing the wrist camera reduced success to 43.3%; removing image-shift augmentation reduced it to 26.7% (Section 4.7).

**Why I care.**

For my SO-101, test camera placement and image augmentation, and evaluate task success rather than validation loss alone.
