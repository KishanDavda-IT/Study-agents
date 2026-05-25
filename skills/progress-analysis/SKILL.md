---
name: progress-analysis
description: >
  Data-driven analysis of the user's learning journey and velocity.
  Use this skill to generate weekly reports or end-of-session summaries.
version: "1.0.0"
metadata:
  category: "Intelligence"
---

# Progress Analysis Skill

## Instructions
1. **Data Aggregation**: Read all files in `/memory/`.
2. **Metric Calculation**: Calculate Retention Rate (%) and Knowledge Velocity (topics/week).
3. **Report Generation**: Use `templates/analysis_report.md` to format the output.

[AGENT_HANDOFF: focus-coach | Action: Milestone_Celebration]
