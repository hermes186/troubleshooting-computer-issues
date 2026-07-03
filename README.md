# Troubleshooting Computer Issues

<<<<<<< HEAD
An agentic skill package for **AI Agent** designed to systematically diagnose and resolve computer configuration errors, software installation issues, network anomalies, and runtime crashes.
=======
An agentic skill package for **AI Agent CLIs (OpenClaw, Gemini CLI, Claude Code)** designed to systematically diagnose and resolve computer configuration errors, software installation issues, network anomalies, and runtime crashes.
>>>>>>> eae723a (update detailed CLI install guides in README)

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

You can install this skill automatically or manually depending on your agent platform:

### 1. For OpenClaw Users
OpenClaw supports direct installation from GitHub or the ClawHub registry:

* **From GitHub (Recommended)**:
  Run this command in your terminal to install the skill globally:
  ```bash
  openclaw skills install git:hermes186/troubleshooting-computer-issues --global
  ```
  *(To install it only for your current project, omit the `--global` flag)*

* **From ClawHub Registry**:
  ```bash
  openclaw skills install @hermes186/troubleshooting-computer-issues --global
  ```
  *(Or if using the standalone `clawhub` CLI: `clawhub install troubleshooting-computer-issues`)*

---

### 2. For Claude Code Users
Claude Code automatically discovers skills placed in its designated skill directories. Clone this repository directly:

* **Global Installation** (available across all projects):
  ```bash
  git clone https://github.com/hermes186/troubleshooting-computer-issues.git ~/.claude/skills/troubleshooting-computer-issues
  ```
* **Project-Specific Installation**:
  Run this inside your project root directory:
  ```bash
  git clone https://github.com/hermes186/troubleshooting-computer-issues.git .claude/skills/troubleshooting-computer-issues
  ```

---

### 3. For Gemini CLI Users
Gemini CLI auto-discovers skills from its config directory or local workspace:

* **Global Installation** (Windows PowerShell):
  ```powershell
  git clone https://github.com/hermes186/troubleshooting-computer-issues.git $env:USERPROFILE\.gemini\config\skills\troubleshooting-computer-issues
  ```
* **Global Installation** (macOS / Linux):
  ```bash
  git clone https://github.com/hermes186/troubleshooting-computer-issues.git ~/.gemini/config/skills/troubleshooting-computer-issues
  ```
* **Project-Specific Installation**:
  Run this inside your project root directory:
  ```bash
  git clone https://github.com/hermes186/troubleshooting-computer-issues.git .agents/skills/troubleshooting-computer-issues
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
