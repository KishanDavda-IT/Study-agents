---
name: learning-style
description: >
  Detects and updates the user's preferred learning style based on behavioral interaction.
  Use this skill whenever the user provides feedback on explanations or demonstrates clear pedagogical preferences.
version: "1.0.0"
metadata:
  category: "Intelligence"
  styles: ["Visual", "Practical", "Theoretical", "Interactive"]
---

# Learning Style Skill

## Instructions
1. **Analyze Interaction**: Detect if the user asks for diagrams (Visual), code (Practical), "why" (Theoretical), or quizzes (Interactive).
2. **Confidence Check**: Only update the profile if the detection confidence is high.
3. **State Update**: Write the detected style to `memory/user_profile.md`.

[AGENT_HANDOFF: memory-maintenance | Action: Sync_Profile]
