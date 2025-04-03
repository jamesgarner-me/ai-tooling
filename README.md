# AI Tooling - Rules Template Repository

This repository contains starter rules files for Cline and Cursor, AI-assisted development tools. These files help structure how these AI tools interact with your projects and maintain context between sessions.

## Contents

- `.clinerules`: Configuration for Cline AI assistant
- `.cursor/`: Configuration for Cursor AI assistant
  - `rules.md`: Main rules file with project-specific guidelines
  - `rules/`: Directory containing modular rule components
    - `core.mdc`: Defines Plan/Act modes of operation
    - `memory-bank.mdc`: Memory bank structure for contextual persistence

## How to Use

### For Cline

1. Copy the `.clinerules` file to the root of your project:

```bash
cp .clinerules /path/to/your/project/
```

2. Create a `/memory-bank` directory in your project root and populate it with the recommended files as described in the rules.

For complete instructions and details, refer to the [official Cline Memory Bank documentation](https://docs.cline.bot/improving-your-prompting-skills/cline-memory-bank).

### For Cursor

1. Copy the `.cursor` directory to the root of your project:

```bash
cp -r .cursor /path/to/your/project/
```

2. Create a `/memory-bank` directory in your project root and populate it with the recommended files as described in the rules.

## Understanding the Memory Bank Concept

The Memory Bank is a structured documentation system that allows AI assistants like Cline and Cursor to maintain context across sessions. It transforms these tools from stateless assistants into persistent development partners that can effectively "remember" your project details over time.

Key benefits include:
- **Context Preservation**: Maintain project knowledge across sessions
- **Consistent Development**: Experience predictable interactions with AI assistants
- **Self-Documenting Projects**: Create valuable project documentation as a side effect
- **Scalable to Any Project**: Works with projects of any size or complexity
- **Technology Agnostic**: Functions with any tech stack or language

Memory Bank files are simply markdown files you create in your project. They're not hidden or special files - just regular documentation stored in your repository that both you and the AI can access.

For more detailed information about the Memory Bank concept, see the [Cline Memory Bank documentation](https://docs.cline.bot/improving-your-prompting-skills/cline-memory-bank).

## Customising for Your Project

### Important Note

The Cursor `rules.md` file contains project-specific placeholders that **must be modified** for your specific project. These placeholders include:

- Language & style preferences
- Documentation standards
- Design principles
- Frontend and backend conventions
- Infrastructure preferences
- Deployment procedures

Review and update these sections to match your project's requirements and conventions before using the rules.

## Memory Bank Structure

Both tools utilise a memory bank approach that maintains context between AI sessions through structured documentation files. The core files include:

- `projectbrief.md`: Core requirements and goals
- `productContext.md`: Purpose and problem definitions
- `systemPatterns.md`: Architecture and design patterns
- `techContext.md`: Technologies and development setup
- `activeContext.md`: Current focus and decisions
- `progress.md`: Status and known issues

To initialize the Memory Bank, create these files with basic content, or ask your AI assistant to "initialize memory bank" and it will help you create the necessary files.

When starting a new session with your AI assistant, use the command "follow your custom instructions" to ensure it reads the Memory Bank files and rebuilds its understanding of your project.

## License

Please see the [LICENSE](LICENSE) file for details. 