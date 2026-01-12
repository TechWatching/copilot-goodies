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
| `feat`     | A new feature (e.g., a new prompt, instruction, or agent) |
| `fix`      | A bug fix                                                |
| `docs`     | Documentation only changes                               |
| `style`    | Code style changes (formatting, missing semi-colons, etc)|
| `refactor` | Code change that neither fixes a bug nor adds a feature  |
| `perf`     | Performance improvements                                 |
| `test`     | Adding or updating tests                                 |
| `build`    | Changes to build system or external dependencies         |
| `ci`       | Changes to CI configuration files and scripts            |
| `chore`    | Other changes that don't modify src or test files        |
| `revert`   | Reverts a previous commit                                |

### 2. Scope (Optional)
- The scope provides additional context about what part of the codebase is affected
- Use lowercase, hyphen-separated words
- Examples: `api`, `auth`, `db`, `ui`, `deps`

### 3. Description
- Use imperative, present tense: "add" not "added" nor "adds"
- Don't capitalize the first letter
- No period at the end
- Keep it concise but descriptive

### 4. Issue Reference (Recommended)
Append the issue or work item number to the commit message using this priority:

1. **From prompt**: Use the issue number if mentioned (e.g., "#123" or "ticket 12345")
2. **From branch name**: Extract from patterns like `feature/123-description` or `bugfix/AB#123-fix` → `#123` or `AB#123`
3. **None found**: Proceed without a reference—do not ask for one

## Examples

```
feat(api): add new endpoint for user export (#123)
fix(db): resolve query timeout issue (#456)
docs(readme): update setup instructions (#789)
refactor(auth): extract validation logic to separate module (#101)
test(api): add integration tests for user endpoints (#202)
chore(deps): update dependencies to latest versions
```