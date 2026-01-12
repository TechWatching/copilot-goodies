# Copilot Goodies

A collection of custom instructions and prompts to enhance your GitHub Copilot experience.

## Overview

This repository contains curated `.instructions.md` and `.prompt.md` files that you can use to customize GitHub Copilot's behavior across your projects. These files help Copilot understand your preferred workflows, coding patterns, and best practices.

## Contents

### 📋 Instructions

Instructions files (`.instructions.md`) define rules and guidelines that Copilot follows when generating or modifying code. They can be applied globally or to specific file patterns.

- **`azure-devops-mcp.instructions.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-instructions%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Finstructions%2Fazure-devops-mcp.instructions.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-instructions%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Finstructions%2Fazure-devops-mcp.instructions.md)
  - Guidelines for working with Azure DevOps MCP Server
  - Work item creation and management best practices
  - Naming conventions and field requirements
  - Linking and relationship management

- **`git-commit.instructions.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-instructions%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Finstructions%2Fgit-commit.instructions.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-instructions%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Finstructions%2Fgit-commit.instructions.md)
  - Conventional Commits specification guidelines
  - Commit type definitions (feat, fix, docs, etc.)
  - Scope and description formatting rules
  - Issue reference recommendations

### 🚀 Prompts

Prompt files (`.prompt.md`) are reusable task templates that guide Copilot through complex multi-step operations.

- **`create-ado-pr.prompt.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Fcreate-ado-pr.prompt.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Fcreate-ado-pr.prompt.md)
  - Creates pull requests on Azure DevOps
  - Auto-extracts work item numbers from commits
  - Generates PR title and description from commit history
  - Supports configurable target branch

- **`init-github-repository.prompt.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Finit-github-repository.prompt.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Finit-github-repository.prompt.md)
  - Automates GitHub repository setup
  - Analyzes workspace and creates appropriate repository
  - Initializes git and pushes code
  - Handles authentication and error scenarios

- **`save-prompt.prompt.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Fsave-prompt.prompt.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-prompt%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fprompts%2Fsave-prompt.prompt.md)
  - Generalizes the current discussion into a reusable prompt
  - Saves the generated prompt to a file

### 🤖 Agents

Agent files (`.agent.md`) define specialized AI agents with specific expertise and capabilities for focused tasks.

- **`custom-agent-creator.agent.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fcustom-agent-creator.agent.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fcustom-agent-creator.agent.md)
  - Specialized agent for creating custom Copilot agents
  - Guides through agent design and configuration
  - Helps define agent capabilities and behavior

- **`microsoft-learn-doc-scout.agent.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fmicrosoft-learn-doc-scout.agent.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fmicrosoft-learn-doc-scout.agent.md)
  - Doc-first research agent using Microsoft Learn MCP server
  - Answers questions with cited Microsoft documentation
  - Covers Azure, .NET, and M365 workloads
  - Provides actionable summaries and guidance

- **`website-retrospec-generator.agent.md`** - [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fwebsite-retrospec-generator.agent.md) [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Install-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode-insiders%3Achat-agent%2Finstall%3Furl%3Dhttps%3A%2F%2Fraw.githubusercontent.com%2Ftechwatching%2Fcopilot-goodies%2Fmain%2Fagents%2Fwebsite-retrospec-generator.agent.md)
  - Generates retrospective analysis for websites
  - Analyzes web architecture and design patterns
  - Provides improvement recommendations

## Installation

### Quick install

Click the **Install in VS Code** or **Install in VS Code Insiders** button next to any instruction, prompt, or agent to install it directly.

### Manual Installation

**To Install:**
- Click the install button above for one-click installation, or
- Download the `*.instructions.md`, `*.prompt.md`, or `*.agent.md` files and manually add them to your VS Code settings

**To Use/Apply:**
- Instructions automatically apply to Copilot behavior once installed
- Prompts can be referenced in Copilot Chat by name
- Agents become available as specialized participants in Copilot Chat

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

### Using Agents

Once installed, custom agents (chat modes) can be selected in the Chat view:

1. Open GitHub Copilot Chat (`Ctrl+Shift+I` or `Cmd+Shift+I`)
2. Select the desired agent from the chat mode dropdown list
3. The agent will respond with its specialized knowledge and capabilities according to its configuration

Custom agents define specialized personas and available tools for specific development tasks like planning, code review, or implementation.

## Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Copilot Instructions Guide](https://code.visualstudio.com/docs/copilot/copilot-customization)

## License

Feel free to use, modify, and share these instructions and prompts. Contributions are welcome!

## Author

Created to enhance developer productivity with GitHub Copilot.

---

**Note**: These instructions and prompts work best with GitHub Copilot Chat in VS Code. Ensure you have the latest version of the GitHub Copilot extension installed.
