---
applyTo: '**'
description: 'Git commit message guidelines'
---

# Git Commit Message Guidelines

## Format

Commit messages **must** follow the [Conventional Commits](https://www.conventionalcommits.org/) specification with an optional issue reference:

```
<type>(<scope>): <description> (#issue)
```

## Rules

### 1. Commit Type (Required)
The type must be one of the following:

| Type       | Description                                              |
|------------|----------------------------------------------------------|
| `feat`     | A new agent, instruction, or prompt                      |
| `fix`      | A fix to an existing agent, instruction, or prompt       |
| `docs`     | Documentation changes (README, LICENSE, etc.)            |
| `style`    | Formatting changes (whitespace, structure, etc.)         |
| `refactor` | Restructuring without changing behavior                  |
| `chore`    | Maintenance tasks (renaming, reorganizing files)         |
| `revert`   | Reverts a previous commit                                |

### 2. Scope (Optional)
- The scope provides additional context about what part of the codebase is affected
- Use lowercase, hyphen-separated words
- Examples: `agents`, `instructions`, `prompts`, `docs`

### 3. Description
- Use imperative, present tense: "add" not "added" nor "adds"
- Don't capitalize the first letter
- No period at the end
- Keep it concise but descriptive

### 4. Issue Reference (Recommended)
Reference the related GitHub issue or Azure DevOps work item at the end of the description:

- Example: `feat(api): add user export endpoint (#123)`

## Examples

```
feat(api): add new endpoint for user export (#123)
fix(db): resolve query timeout issue (#456)
docs(readme): update setup instructions (#789)
refactor(auth): extract validation logic to separate module (#101)
test(api): add integration tests for user endpoints (#202)
chore(deps): update dependencies to latest versions
```