# Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation

**Authors / year:** Zipeng Fu, Tony Z. Zhao, Chelsea Finn / 2024
**Link:** https://arxiv.org/abs/2401.02117
**PDF:** [Local copy](<../../Zotero/storage/HA6KJW7N/Fu et al. - 2024 - Mobile ALOHA Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation.pdf>)
**Zotero:** [Item](zotero://select/library/items/LNJQ3TW4) · [Read PDF](zotero://open-pdf/library/items/HA6KJW7N)
**Batch:** 2 — imitation learning for manipulation (paper 6)
**Read on:** 10/27/2026

**Problem.** What were they unable to do before this paper?

Most imitation learning focused on tabletop tasks; everyday tasks require coordinating two arms and a mobile base with limited demonstration data.

**Method.** In two or three sentences. What is the actual mechanism?

They added a wheeled base and whole-body teleoperation to ALOHA, then trained ACT to predict arm and base action chunks together. Training mixes mobile-task demonstrations equally with existing static ALOHA data, adding zero base velocities to the static actions.

**Result.** The number that matters, and on what task.

On Wipe Wine, co-training achieved 95% success versus 50% without it, using 50 mobile-task demonstrations plus 825 static demonstrations. Each condition had 20 evaluation trials (Table 1).

**Why I care.** One line — how it connects to the SO-101 or to sim-to-real.

For my SO-101, test whether compatible demonstrations from other tasks improve ACT over target-task data alone.
