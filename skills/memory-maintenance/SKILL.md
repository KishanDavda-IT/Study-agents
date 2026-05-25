---
name: memory-maintenance
description: >
  System maintenance skill to keep the Study-Agents memory files lean and high-signal.
  Use this skill at the end of every session or when the ledger exceeds 20 rows.
version: "1.0.0"
metadata:
  category: "System"
---

# Memory Maintenance Skill

## Instructions
1. **Archive Check**: Move topics with Confidence > 9 to `memory/archive_ledger.md`.
2. **Compress Notes**: Summarize detailed interaction notes in `subject_ledger.md` into single-line "Key Insights."
3. **Prune**: Remove empty rows or redundant session log entries.

[AGENT_HANDOFF: progress-analysis | Action: Final_Report]
