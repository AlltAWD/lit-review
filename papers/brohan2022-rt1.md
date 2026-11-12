# RT-1: Robotics Transformer for Real-World Control at Scale

**Authors / year:** Anthony Brohan, Noah Brown, Justice Carbajal, et al. / 2022
**Link:** https://arxiv.org/abs/2212.06817
**PDF:** [Local copy](<../../Zotero/storage/PK9G7AF5/Brohan et al. - 2022 - RT-1 Robotics Transformer for Real-World Control at Scale.pdf>)
**Zotero:** [Item](zotero://select/library/items/UC8VIGK5) · [Read PDF](zotero://open-pdf/library/items/PK9G7AF5)
**Batch:** 4 — the map, then where the field is now (paper 11)
**Read on:** 10/28/2026

**Problem.** What were they unable to do before this paper?

Robot policies trained on narrow task datasets generalize poorly to new instructions, objects, and environments.

**Method.** In two or three sentences. What is the actual mechanism?

They train one language-conditioned policy on roughly 130,000 demonstrations covering over 700 instructions. RT-1 compresses image features conditioned on the instruction into tokens, then uses a Transformer to predict discretized arm and base actions, controlling the robot at 3 Hz.

**Result.** The number that matters, and on what task.

RT-1 achieved 97% success on seen-task evaluations and 76% on 21 unseen instructions combining familiar skills and objects in new ways (Table 2).

**Why I care.**

For my SO-101, this motivates collecting diverse tasks with clear language labels to test generalization beyond a single routine.
