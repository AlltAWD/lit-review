# Sim-to-Real Transfer of Robotic Control with Dynamics Randomization

**Authors / year:** Xue Bin Peng, Marcin Andrychowicz, Wojciech Zaremba, Pieter Abbeel / 2018
**Link:** https://arxiv.org/abs/1710.06537
**PDF:** [Local copy](<../../Zotero/storage/BIH8UATP/Peng et al. - 2018 - Sim-to-Real Transfer of Robotic Control with Dynamics Randomization.pdf>)
**Zotero:** [Item](zotero://select/library/items/M53YQC9W) · [Read PDF](zotero://open-pdf/library/items/BIH8UATP)
**Batch:** 3 — sim-to-real for control (paper 7)
**Read on:** 10/28/2026

**Problem.** What were they unable to do before this paper?

Control policies trained in simulation often fail on real robots because simulated masses, friction, and actuator behavior differ from reality.

**Method.** In two or three sentences. What is the actual mechanism?

They train a recurrent reinforcement-learning policy while randomizing physical parameters, controller timing, and observation noise in simulation. The policy uses observation history to adapt to unfamiliar dynamics, then runs on the real robot without further training.

**Result.** The number that matters, and on what task.

On a real Fetch arm, the policy pushed a puck within 7 cm of its target with 89% success over 28 trials, compared with 91% in simulation (Table II).

**Why I care.** One line — how it connects to the SO-101 or to sim-to-real.

For my SO-101, randomizing physics and control timing could help a Gazebo-trained policy tolerate imperfect calibration.
