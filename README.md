# Mistral OCR Skill

> A universal AI agent skill for extracting structured text, tables, and document layouts using Mistral OCR capabilities.

## 📦 Installation

This skill is designed to be agent-agnostic. It works with any AI coding assistant that supports local skill directories (OpenCode, Cursor, Claude Code, Cline, GitHub Copilot, etc.).

### Option 1: Universal Local Install (Recommended)
Clone this repository directly into your agent's local skills directory. This method works everywhere and requires no marketplace registration.

```bash
git clone https://github.com/rexTexTau/mistral-ocr.git ~/.agents/skills/mistral-ocr
```

*(Note: Adjust `~/.agents/skills/` to match your specific agent's expected directory if different, e.g., `~/.cursor/skills/` or `~/.config/opencode/skills/`)*

### Option 2: Agent-Native Commands
If your agent supports direct GitHub repository installation, you can use its native command:
- **OpenCode**: `opencode skill add rexTexTau/mistral-ocr`
- **Claude Code**: `/plugin add rexTexTau/mistral-ocr`
- **Cursor / Cline**: Manually copy or symlink this repo into `.cursor/skills/mistral-ocr` or `.cline/skills/mistral-ocr`

## 🚀 Usage
Once installed, your AI agent will automatically load this skill's context. You can invoke it naturally:
- "Use the mistral-ocr skill to extract all tables from this book page photo."
- "Run the mistral-ocr recipe to analyze the layout of this scanned document."

## 📂 Repository Structure
- `SKILL.md` / `AGENTS.md`: Core instructions, rules, and context for the AI agent.
- `recipes/`: Pre-defined workflows and prompt templates for common OCR tasks.
- `scripts/`: Helper scripts to automate OCR processing pipelines.

## 🔄 Updating
To update the skill to the latest version, simply pull the latest changes:
```bash
git -C ~/.agents/skills/mistral-ocr pull
# Or for project-local: git -C .agents/skills/mistral-ocr pull
```
