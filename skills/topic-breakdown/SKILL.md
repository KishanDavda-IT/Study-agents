---
name: topic-breakdown
description: >
  Deconstructs complex or technical topics into their fundamental "First Principles" components.
  Use this skill when the user introduces a new subject, asks "How does X work?", or needs a learning roadmap.
version: "1.0.0"
metadata:
  category: "Pedagogy"
  handoff_target: "concept-simplifier"
---

# Topic Breakdown Skill

## Overview
This skill implements the initial "Structural Breakdown" phase of the learning workflow. It ensures that any topic, no matter how complex, is reduced to 3-5 manageable logical blocks.

## Instructions
1. **Analyze Subject**: Identify the core technical domain of the requested topic.
2. **First Principles Extraction**: Strip away high-level abstractions to find the foundational concepts.
3. **Deconstruction**:
   - Create 3-5 distinct sub-topics.
   - Sequence them such that each builds upon the previous one.
   - Use clear, non-jargon headings.
4. **Verification**: Present the breakdown to the user and ask for approval before proceeding to explanation.

## Contextual Integration
- **Context Source**: Read `memory/user_profile.md` to adjust technical depth.
- **State Update**: Suggest an update to `memory/subject_ledger.md` once the breakdown is finalized.

## Output Format
Always start with a brief "Hook" explaining the topic's importance, followed by a bulleted list of the breakdown components.

[AGENT_HANDOFF: concept-simplifier | Topic: [First_Component] | Style: [User_Preferred]]
