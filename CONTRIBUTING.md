# Contributing to Awesome OpenCode Subagents

Thank you for your interest in contributing to this collection! This repository is a pure content hub for OpenCode subagents, managed and searchable via the **opencoding-agent** plugin.

## 🤝 How to Contribute

### Adding a New Subagent

1.  **Choose the right category** - Place your subagent in the most appropriate category folder under `categories/`.
2.  **Test your subagent** - Ensure it works with OpenCode and follows the YAML frontmatter specification.
3.  **Update required files** - When adding a new agent, you must update:
    - **Main README.md**: Add your agent link in the appropriate category section (alphabetical order).
    - **Category README.md**: Add a detailed description in the "Available Subagents" section and update the selection guide table.
    - **Your agent .md file**: Create the actual agent definition following the template in `AGENT_GUIDE.md`.
4.  **Regenerate Catalog** - Run the catalog generator tool (if you have local access) or let the maintainers handle it during PR review to update `catalog.json`.
5.  **Submit a PR** - Include a clear description of the subagent's purpose.

### Subagent Requirements

Each subagent should include:
- Clear role definition
- List of expertise areas
- OpenCode-compliant YAML frontmatter
- Communication protocol examples (JSON)
- Core capabilities
- Example usage scenarios
- Best practices

### Pull Request Process

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/new-subagent`).
3.  Add your subagent following the template.
4.  Update ALL required locations:
    - Main README.md (alphabetical order).
    - Category-specific README.md.
5.  Verify all links work correctly.
6.  Submit a pull request with a clear description.

### Quality Guidelines

- Subagents should be well-structured and provide high-value instructions.
- Ensure compatibility with OpenCode tool names and formats.
- Provide practical, executable examples in the description.

## 📝 License

By contributing, you agree that your contributions will be licensed under the MIT License.

All subagents in this repository are provided "as is" without warranty. The maintainers do not audit or guarantee the security or correctness of any contribution and accept no liability for any issues arising from their use.
