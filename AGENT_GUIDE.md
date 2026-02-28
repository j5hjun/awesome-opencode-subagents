# OpenCode Subagent Creation Guide

This guide explains how to create and contribute new subagents to this repository.

## 1. File Structure

All subagents should be placed in the appropriate directory under `categories/`. If you're creating a new category, follow the existing numbering convention (e.g., `11-new-category`).

## 2. Agent Format

Each agent must be a Markdown file with the following YAML frontmatter structure:

```yaml
---
description: >-
  Detailed description of when this agent should be invoked. 
  This is used by the LLM to decide which subagent to spawn.
mode: subagent
tools:
  bash: true
  read: true
  write: true
  edit: true
  list: true
  glob: true
  grep: true
  webfetch: false
  task: false
  todowrite: true
  todoread: true
---

# Role Name
You are an expert in...

## Responsibilities
- Task A
- Task B

## Workflow
1. Analyze...
2. Implement...
```

### Tool Selection
- **read-only**: `read`, `glob`, `grep`
- **developer**: `read`, `write`, `edit`, `bash`, `glob`, `grep`, `todowrite`, `todoread`
- **researcher**: `read`, `glob`, `grep`, `webfetch`

## 3. Communication Protocol

Subagents should include a JSON-based communication section if they are expected to collaborate with other agents.

```json
{
  "requesting_agent": "agent-name",
  "request_type": "get_context",
  "payload": { "query": "..." }
}
```

## 4. Submission Process

1. Fork the repository.
2. Add your `.md` file to the correct category.
3. Update the category's `README.md` if necessary.
4. Run the catalog generator (internal tool) to update `catalog.json`.
5. Submit a Pull Request.
