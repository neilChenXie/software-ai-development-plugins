# Software AI Development Plugins

A collection of AI-powered plugins and skills for software development, designed to enhance productivity in Claude Code, OpenCode, and similar AI coding assistants.

## Overview

This project provides a suite of tools that help developers:

- **Generate documentation** (README, code comments, dev logs) automatically
- **Learn projects** through structured, project-based learning plans
- **Record sessions** for later review and knowledge extraction

## Plugins

### [development-doc-tools](plugins/development-doc-tools)

A plugin for software development documentation, including:

| Skill | Description |
|-------|-------------|
| `generate-readme` | Generate README.md files for projects or individual files |
| `generate-code-comment` | Auto-generate code comments with function purpose and parameter explanations |
| `generate-dev-logs` | Summarize daily development logs from conversation records |
| `project-based-learn` | Create structured learning plans based on project codebases |

### External Plugins

| Plugin | Description | Source |
|--------|-------------|--------|
| `claude-session-recorder` | Automatically generates Markdown logs of Claude Code session transcripts | [GitHub](https://github.com/neilChenXie/claude-session-recorder) |
| `api-tools-knowledge` | Software development knowledge base including API docs, SDKs, IoT protocols, and code examples | [GitHub](https://github.com/neilChenXie/api-tools-knowledge) |

## Installation

### For Claude Code

Add the marketplace and install plugins via CLI:

```bash
# Add this plugin marketplace
claude plugin marketplace add neilChenXie/software-ai-development-plugins

# Install the plugin (user scope by default)
claude plugin install development-doc-tools@software-ai-development-plugins

# Or install to project scope (shared with team)
claude plugin install development-doc-tools@software-ai-development-plugins --scope project
```

Then run `/reload-plugins` in your Claude Code session to activate the plugin.

### For OpenCode / Other Agents

Clone the repository and symlink the skills directory:

```bash
git clone https://github.com/neilChenXie/software-ai-development-plugins.git ~/.agents/skills/software-ai-development-plugins

# In your agent's config directory:
ln -s ~/.agents/skills/software-ai-development-plugins/plugins/development-doc-tools/skills ./skills
```

## Project Structure

```
software-ai-development-plugins/
├── .claude-plugin/
│   └── marketplace.json          # Plugin marketplace manifest
├── plugins/
│   └── development-doc-tools/    # Core documentation plugin
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           ├── generate-code-comment/
│           ├── generate-dev-logs/
│           ├── generate-readme/
│           └── project-based-learn/
├── conversations/                # Session conversation records
├── hooks/                          # Git hooks
└── README.md                       # This file
```

## Author

**Chen Xie** — [chenxie121@gmail.com](mailto:chenxie121@gmail.com)

## License

MIT
