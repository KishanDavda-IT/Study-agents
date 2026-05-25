---
name: revision
description: >
  Manages Spaced Repetition (SRS) and long-term retention. 
  Use this skill to schedule review sessions and calculate confidence decay for learned topics.
version: "1.1.0"
metadata:
  system: "Spaced Repetition"
  feature: "Confidence Decay"
---

# Revision Skill

## Instructions
1. **Log Audit**: Read `memory/revision_log.md` and `memory/subject_ledger.md`.
2. **Decay Calculation**: 
   - Identify topics overdue for review.
   - Apply Confidence Decay penalties based on the delay (3 days = -1 point, 7 days = -3 points).
3. **Scheduling**:
   - For successful reviews, increment the interval (1 -> 3 -> 7 -> 14 -> 30 days).
   - For failed reviews, reset the interval to 1 day and flag the topic as "At-Risk."

## Verification
Prompt the user with a "Check for Understanding" question from a previous session to verify retention before updating the log.

[AGENT_HANDOFF: progress-analysis | Action: Update_Retention_Stats]
