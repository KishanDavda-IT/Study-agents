# Study-Agents

A production-ready, pure markdown-driven AI agent workflow project designed for autonomous AI development environments (Claude Code, Cursor, Roo Code, OpenCode).

## Overview

Study-Agents is not a chatbot. It is a modular system of autonomous study-focused agents that operate through structured prompts, instruction files, and persistent memory. It functions as an AI-powered study operating system.

## Architecture

- **`/agents`**: Instruction files (AIFs) defining specific agent personas and logic.
- **`/memory`**: Persistent state tracking learning styles, progress, and revision schedules.
- **`/templates`**: Standardized output schemas for interoperability.
- **`/workflows`**: Orchestration logic for complex multi-agent tasks.

## Getting Started

To use Study-Agents, point your agentic AI IDE (like Claude Code) to this directory. The system is self-documenting via `SYSTEM_INSTRUCTIONS.md`.

## Core Agents

- `topic-breakdown-agent`: Simplifies complex topics.
- `learning-style-agent`: Adapts to user preferences.
- `study-planner-agent`: Manages goals and roadmaps.
- `revision-agent`: Handles spaced repetition.
- `quiz-agent`: Generates active recall exercises.
- `progress-analysis-agent`: Tracks and improves performance.
- `focus-coach-agent`: Maintains discipline and motivation.
- `concept-simplifier-agent`: Re-explains concepts from different angles.
