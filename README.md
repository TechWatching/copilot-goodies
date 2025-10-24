# Copilot Goodies

A collection of custom instructions and prompts to enhance your GitHub Copilot experience.

## Overview

This repository contains curated `.instructions.md` and `.prompt.md` files that you can use to customize GitHub Copilot's behavior across your projects. These files help Copilot understand your preferred workflows, coding patterns, and best practices.

## Contents

### 📋 Instructions

Instructions files (`.instructions.md`) define rules and guidelines that Copilot follows when generating or modifying code. They can be applied globally or to specific file patterns.

- **`azure-devops-mcp.instructions.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode:chat-instructions/install?url=https://raw.githubusercontent.com/techwatching/copilot-goodies/main/instructions/azure-devops-mcp.instructions.md)
  - Guidelines for working with Azure DevOps MCP Server
  - Work item creation and management best practices
  - Naming conventions and field requirements
  - Linking and relationship management

### 🚀 Prompts

Prompt files (`.prompt.md`) are reusable task templates that guide Copilot through complex multi-step operations.

- **`init-github-repository.prompt.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode:chat-prompt/install?url=https://raw.githubusercontent.com/techwatching/copilot-goodies/main/prompts/init-github-repository.prompt.md)
  - Automates GitHub repository setup
  - Analyzes workspace and creates appropriate repository
  - Initializes git and pushes code
  - Handles authentication and error scenarios

## Installation

### Quick install

Click the **Install in VS Code** button next to any instruction or prompt to install it directly.

### Manual Installation

**To Install:**
- Click the install button above for one-click installation, or
- Download the `*.instructions.md` or `*.prompt.md` files and manually add them to your VS Code settings

**To Use/Apply:**
- Instructions automatically apply to Copilot behavior once installed
- Prompts can be referenced in Copilot Chat by name

### Alternative: Workspace-Specific Setup

You can also add these files to individual workspaces by placing them in your workspace's `.github/instructions` folder.

## Usage

### Using Instructions

Once installed, instructions are automatically applied based on their `applyTo` frontmatter:

```markdown
---
description: 'Guidelines for using Azure DevOps MCP Server'
applyTo: '**'
---
```

- `**` applies to all files in the workspace
- Specific patterns like `*.ts` apply only to TypeScript files

### Using Prompts

Prompts can be invoked in Copilot Chat:

1. Open GitHub Copilot Chat (`Ctrl+Shift+I` or `Cmd+Shift+I`)
2. Reference the prompt by name or use the prompt picker
3. Copilot will follow the steps defined in the prompt

Example:
```
@workspace Use the init-github-repository prompt to set up this project
```

## Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Copilot Instructions Guide](https://code.visualstudio.com/docs/copilot/copilot-customization)

## License

Feel free to use, modify, and share these instructions and prompts. Contributions are welcome!

## Author

Created to enhance developer productivity with GitHub Copilot.

---

**Note**: These instructions and prompts work best with GitHub Copilot Chat in VS Code. Ensure you have the latest version of the GitHub Copilot extension installed.
