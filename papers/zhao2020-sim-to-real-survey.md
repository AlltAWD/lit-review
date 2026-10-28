# Sim-to-Real Transfer in Deep Reinforcement Learning for Robotics: a Survey

**Authors / year:** Wenshuai Zhao, Jorge Peña Queralta, Tomi Westerlund / 2020
**Link:** https://arxiv.org/abs/2009.13303
**PDF:** [Local copy](<../../Zotero/storage/LKRKHX8C/Zhao et al. - 2020 - Sim-to-Real Transfer in Deep Reinforcement Learning for Robotics a Survey.pdf>)
**Zotero:** [Item](zotero://select/library/items/CDACGT27) · [Read PDF](zotero://open-pdf/library/items/LKRKHX8C)
**Batch:** 4 — the map, then where the field is now (paper 10)
**Read on:** 10/28/2026

**Reading note:** This is a survey: use its section headings as a map for synthesis.md. For Result, record the scope or taxonomy rather than inventing an experimental success rate.

**Problem.** What were they unable to do before this paper?

Simulation makes robot learning cheaper, but mismatches in sensing and dynamics hinder transfer. Existing approaches lacked a unified review explaining their relationships.

**Method.** In two or three sentences. What is the actual mechanism?

They review published studies, comparing transfer methods, simulators, learning algorithms, robots, and tasks. They distinguish domain randomization, which varies training environments for robustness, from domain adaptation, which aligns source and target domains.

**Result.** The number that matters, and on what task.

Maps five approaches—domain randomization, domain adaptation, imitation learning, meta-learning, and knowledge distillation—across manipulation, navigation, and other applications. The contribution is a taxonomy, not a new experimental success rate (Sections II–IV; Table I).

**Why I care.** One line — how it connects to the SO-101 or to sim-to-real.

I can use this map to organize synthesis.md and separate visual-transfer methods from dynamics-transfer methods for my SO-101.
