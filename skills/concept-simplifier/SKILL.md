---
name: concept-simplifier
description: >
  Converts technical topics into intuitive, easy-to-grasp explanations using analogies and metaphors.
  Use this skill when the user is confused, requests an "ELI5," or after a topic breakdown has been established.
version: "1.0.0"
metadata:
  category: "Pedagogy"
  features: ["Dynamic Reframing", "Analogy Generation"]
---

# Concept Simplifier Skill

## Overview
The goal of this skill is to achieve conceptual clarity. It bridges the gap between technical rigor and intuitive understanding through vivid storytelling and structural analogies.

## Instructions
1. **Misconception Audit**: Check if the user's inquiry contains technical flaws.
2. **Reframing (Self-Correction)**: If flawed, explain the error first, then pivot to the correct principle.
3. **Analogy Generation**:
   - Consult `memory/user_profile.md` for the user's preferred analogy domain (e.g., Code, Cooking, Sports).
   - Create a vivid metaphor that maps 1:1 to the technical concept.
4. **The "Skeleton" Explanation**: Provide the technical details step-by-step, anchored to the analogy.

## Dynamic Reframing Rules
- If the question is "not good" or logically broken:
  - **Acknowledge** the intent.
  - **Reframe** into a productive learning path.
  - **Teach** the fundamental before answering.

## Output Format
Follow the `templates/explanation_format.md` structure:
- Analogy Block
- Explanation Block
- Key Takeaway
- Hands-on Example
- Check for Understanding

[AGENT_HANDOFF: quiz-agent | Topic: [Current_Topic] | Context: [Last_Explanation]]
