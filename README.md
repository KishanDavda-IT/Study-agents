# Study-Agents 🧠

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Architecture](https://img.shields.io/badge/Architecture-Agent%20Skills-green.svg)](https://github.com/anthropics/skills)

**Study-Agents** is a professional, modular, and markdown-first autonomous AI study framework. It transforms agentic AI IDEs (like Claude Code, Cursor, and Roo Code) into a self-evolving "Study Operating System" that orchestrates a team of specialized pedagogical agents to help you master any topic.

---

## 🚀 Key Features

*   **Professional "Agent Skills" Architecture**: Built on the Anthropic `SKILL.md` standard. Each agent is a discrete, discoverable skill with YAML metadata and imperative instructions.
*   **🎨 Visual Engine (Mermaid.js)**: Agents autonomously generate logical flowcharts and mind maps for complex topics, providing instant visual clarity.
*   **📡 Real-Time Research**: Mandated web-research steps for fast-moving fields (AI, Space, Medicine) to ensure pedagogical accuracy and latest breakthroughs.
*   **🛡️ Self-Correcting Logic**: Agents detect flawed user inquiries and misconception-based questions, reframing them into productive learning paths before answering.
*   **📉 Confidence Decay & SRS**: A realistic Spaced Repetition System that tracks retention and penalizes confidence scores if review sessions are missed.
*   **🧹 Memory Maintenance**: Automated agents that prune context, archive mastered topics, and keep your "Study OS" lean and high-signal.

---

## 📂 Core Structure

```text
Study-Agents/
├── SYSTEM_INSTRUCTIONS.md    # The "Orchestrator" brain & core rules
├── skills/                   # Professional Agent Skill library
│   ├── topic-breakdown/      # Deconstructs topics into First Principles
│   ├── concept-simplifier/   # ELI5 + Vivid Analogies + Mermaid Diagrams
│   ├── revision/             # SRS Management & Confidence Decay logic
│   ├── onboarding/           # Interactive user-profile setup
│   └── ... (9 specialized skills)
├── memory/                   # Persistent SRS, Progress, and Profile state
├── workflows/                # Multi-skill autonomous orchestration scripts
└── templates/                # Standardized output interfaces
```

---

## 🛠️ Getting Started

### 1. Installation
Simply clone this repository into your project workspace:
```bash
git clone https://github.com/KishanDavda-IT/Study-agents.git
```

### 2. Activation
Point your agentic AI IDE (Claude Code, Cursor, Roo Code) to this directory. The system is designed to be self-discovering via the `SYSTEM_INSTRUCTIONS.md`.

### 3. Usage Examples
*   **Initialize**: `/ask Start the onboarding process.`
*   **Learn**: `/ask I want to learn about Quantum Field Theory.`
*   **Revision**: `/ask What should I review today?`
*   **Analysis**: `/ask Show me my progress report.`

---

## 🤝 Contributing
This is an open-source project. We welcome contributions to new specialized skills (e.g., Coding-Tutor, Language-Immersion) and improvements to our SRS algorithms.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Built for the next generation of autonomous AI learning ecosystems.*
