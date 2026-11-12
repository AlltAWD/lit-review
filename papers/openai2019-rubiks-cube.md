# Solving Rubik's Cube with a Robot Hand

**Authors / year:** OpenAI, Ilge Akkaya, Marcin Andrychowicz, et al. / 2019
**Link:** https://arxiv.org/abs/1910.07113
**PDF:** [Local copy](<../../Zotero/storage/NKEF66G2/OpenAI et al. - 2019 - Solving Rubik's Cube with a Robot Hand.pdf>)
**Zotero:** [Item](zotero://select/library/items/H4YJE5WB) · [Read PDF](zotero://open-pdf/library/items/NKEF66G2)
**Batch:** 3 — sim-to-real for control (paper 8)
**Read on:** 10/28/2026

**Reading note:** Read only the abstract and the automatic domain randomization (ADR) section on this pass, as specified in the reading plan.

**Problem.** What were they unable to do before this paper?

Fixed randomization ranges require manual tuning and may not cover the variation needed for complex real-world dexterous manipulation.

**Method.** In two or three sentences. What is the actual mechanism?

Automatic domain randomization (ADR) expands parameter ranges when boundary tests succeed and contracts them when performance falls. They train a recurrent controller and a vision model in simulation; a conventional cube solver supplies the move sequence.

**Result.** The number that matters, and on what task.

With vision for cube pose and sensor-measured face angles, the best policy completed the fixed scramble sequence of 26 rotations and 17 flips in 2 of 10 real-hand trials (Table 6).

**Why I care.**

For my SO-101, progressively expanding randomization could improve robustness without choosing every training range by hand.
