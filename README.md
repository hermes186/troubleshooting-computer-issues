# Troubleshooting Computer Issues

An agentic skill package for **AI Agent** designed to systematically diagnose and resolve computer configuration errors, software installation issues, network anomalies, and runtime crashes.

---

## 🚀 Features

- **Dynamic Difficulty Classification**: Automatically classifies issues into 4 levels (Simple, Medium, Hard, Extreme) and dynamically scales diagnostic depth or adjusts classifications based on evidence.
- **Cross-Platform Diagnostic Commands**: Standardized command matrices for Windows (PowerShell), macOS, and Linux to trace ports, process state, paths, and logs.
- **Isolated Troubleshooting Memory**: Automatically initializes a local `.troubleshooting-memory/` directory to write solved cases (`SOLUTIONS.md`), unresolved attempts (`UNRESOLVED.md`), and extract recurring patterns (`PATTERNS.md`).
- **Completely Self-Contained**: Optimized using relative paths, making it ready to be published and shared.

---

## 📁 Directory Structure

```text
troubleshooting-computer-issues/
├── SKILL.md                          # Core flow & logic
├── README.md                         # This instruction file
└── references/                       # Detailed reference manuals
    ├── diagnostic-templates.md       # Diagnostic checklists & commands
    ├── memory-format.md              # Troubleshooting memory schema
    └── common-solutions.md           # Quick solution index for common errors
```

---

## 🛠️ Installation & Usage

### Via ClawHub (Recommended)
This skill is officially published on ClawHub! You can install it automatically using:

```bash
clawhub install hermes186/troubleshooting-computer-issues
```

Detailed page: [troubleshooting-computer-issues on ClawHub](https://clawhub.ai/hermes186/skills/troubleshooting-computer-issues)

### Manual Installation
Clone or copy this folder directly into your global agent skills directory:

```bash
# Example for Gemini / OpenClaw global skills directory
cp -r troubleshooting-computer-issues ~/.gemini/config/skills/
```

---

## 🧠 Memory Integration

When this skill resolves an issue, it creates a local directory `.troubleshooting-memory/` in the project root:

- **SOLUTIONS.md**: Stores successfully resolved cases with root cause analysis.
- **UNRESOLVED.md**: Records failed attempts and blockers to prevent duplicate trial-and-error.
- **PATTERNS.md**: Consolidates repetitive errors (occurring 3+ times) into rapid-lookup patterns.

---

## 📄 License

Licensed under the **MIT License**.
