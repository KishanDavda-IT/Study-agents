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
1. **Real-Time Research**: If the topic is in a fast-moving field (e.g., LLMs, Space Exploration), perform a web search to identify the latest developments or state-of-the-art information.
2. **Analyze Subject**: Identify the core technical domain.
3. **First Principles Extraction**: Strip away high-level abstractions.
4. **Deconstruction**:
   - Create 3-5 distinct sub-topics.
5. **Visual Mapping (Visual Engine)**:
   - Generate a **Mermaid.js** `graph TD` block showing the logical relationship between the sub-topics.
6. **Verification**: Present the breakdown and diagram to the user.

## Output Format
Always start with a brief "Hook", followed by the **Mermaid.js diagram**, then the bulleted list. Cite the latest research source if applicable.

[AGENT_HANDOFF: concept-simplifier | Topic: [First_Component] | Style: [User_Preferred]]

