---
name: onboarding
description: >
  Professional first-run experience to initialize the user's learning profile and goals.
  Use this skill when the user first starts the system or if the 'user_profile.md' is empty.
version: "1.0.0"
metadata:
  category: "System"
  priority: "High"
---

# Onboarding Skill

## Overview
This skill guides the user through a structured "Interview" to establish their learning baseline, preferences, and long-term goals.

## Instructions
1. **Detect State**: Check if `memory/user_profile.md` contains "Unknown" or default values.
2. **The Interview**:
   - Ask for the user's **primary learning goal** (e.g., "I want to learn Deep Learning for my job").
   - Determine **Learning Style**: Present 3 options (Visual, Practical, Theoretical).
   - Establish **Session Cadence**: Ask for preferred session length.
3. **Profile Generation**:
   - Synthesize the answers.
   - Update `memory/user_profile.md` with the new data.
4. **First Step**: Immediately hand off to the `study-planner` to create a roadmap.

## Tone
- Welcoming.
- Expert.
- Encouraging.

[AGENT_HANDOFF: study-planner | Action: Initial_Roadmap]
