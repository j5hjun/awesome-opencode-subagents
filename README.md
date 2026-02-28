<a href="https://github.com/j5hjun/awesome-opencode-subagents">
<img width="1500" height="500" alt="Awesome OpenCode Subagents" src="https://github.com/user-attachments/assets/55b97c47-8506-4be0-b18f-f5384d063cbb" />
</a>

<br />
<br/>

<div align="center">
    <strong>The awesome collection of OpenCode subagents.</strong>
    <br />
    <br />
</div>

<div align="center">
    
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Subagent Count](https://img.shields.io/badge/subagents-130-blue?style=flat-square)
[![Last Update](https://img.shields.io/github/last-commit/j5hjun/awesome-opencode-subagents?label=Last%20update&style=flat-square)](https://github.com/j5hjun/awesome-opencode-subagents)
[![GitHub forks](https://img.shields.io/github/forks/j5hjun/awesome-opencode-subagents?style=social)](https://github.com/j5hjun/awesome-opencode-subagents/network/members)
    
</div>

# Awesome OpenCode Subagents 

This repository is the definitive collection of OpenCode subagents—specialized AI assistants refactored specifically for the OpenCode ecosystem. These agents are designed to handle complex development, infrastructure, and research tasks with precision.

## 🚀 How to Use

The best way to browse and install these subagents is using the **[opencoding-agent](https://github.com/j5hjun/opencoding-agent)** plugin.

### 1. Install the Plugin
Ensure you have the `opencoding-agent` plugin installed in your OpenCode environment.

### 2. Browse & Install Agents
Use the following commands within OpenCode:

*   `/subagent-catalog:list` - Browse categories and agents.
*   `/subagent-catalog:search <query>` - Search for a specific expert (e.g., `php`, `security`).
*   `/subagent-catalog:fetch <name>` - Download and install the agent definition to your local environment.

---

## 📚 Categories

### [01. Core Development](categories/01-core-development/)
Essential development subagents for everyday coding tasks.
- [**api-designer**](categories/01-core-development/api-designer.md) - REST and GraphQL API architect
- [**backend-developer**](categories/01-core-development/backend-developer.md) - Server-side expert for scalable APIs
- [**frontend-developer**](categories/01-core-development/frontend-developer.md) - UI/UX specialist for React, Vue, and Angular
- [**fullstack-developer**](categories/01-core-development/fullstack-developer.md) - End-to-end feature development
- ... (See category for more)

### [02. Language Specialists](categories/02-language-specialists/)
Language-specific experts with deep framework knowledge.
- [**typescript-pro**](categories/02-language-specialists/typescript-pro.md) - TypeScript specialist
- [**python-pro**](categories/02-language-specialists/python-pro.md) - Python ecosystem master
- [**rust-engineer**](categories/02-language-specialists/rust-engineer.md) - Systems programming expert
- ... (See category for more)

### [03. Infrastructure](categories/03-infrastructure/)
DevOps, cloud, and deployment specialists.
- [**kubernetes-specialist**](categories/03-infrastructure/kubernetes-specialist.md) - Container orchestration master
- [**terraform-engineer**](categories/03-infrastructure/terraform-engineer.md) - Infrastructure as Code expert
- ... (See category for more)

*(Full list available in the [Catalog](catalog.json))*

---

## 🛠 Subagent Format

Every agent in this repository follows the OpenCode YAML frontmatter specification:

```yaml
---
description: Brief description of the agent's purpose
mode: subagent
tools:
  read: true
  write: true
  bash: true
  ...
---
System prompt follows...
```

---

## 🤝 Contributing

Contributions are welcome! Please see [AGENT_GUIDE.md](AGENT_GUIDE.md) for instructions on how to create and submit new OpenCode subagents.

## 📄 License

MIT License - see [LICENSE](LICENSE)

This repository is a curated collection provided "as is". Review agents before use; the maintainers accept no liability for issues arising from their use.
