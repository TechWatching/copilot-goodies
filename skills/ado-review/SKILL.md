---
name: ado-review
description: >
  Review an Azure DevOps pull request. Use when the user invokes /ado-review <PR-ID>
  or asks for an Azure DevOps PR review.
argument-hint: "<PR-ID>"
---

# Azure DevOps Pull Request Review (Template)

## Project Context

Retrieve the project/repo identifiers.

## Review Process

### 1) Resolve PR and repository

- Extract PR ID from user input.
- Query PRs in project `<PROJECT>` to find matching ID.
- Capture repository name and ID from the result.

### 2) Fetch PR metadata

- Retrieve title, description, author, source/target branches, reviewers, status, linked work items.

### 3) Get diff via local git

Map ADO repo names to local paths, for example:

| ADO repo name | Local path |
|---|---|
| `<REPO_A>` | `C:\dev\<WORKSPACE>\<REPO_A>` |
| `<REPO_B>` | `C:\dev\<WORKSPACE>\<REPO_B>` |

Run:

```powershell
git fetch origin
git diff --name-status origin/<targetBranch>...origin/<sourceBranch>
git diff origin/<targetBranch>...origin/<sourceBranch>
```

### 4) Review dimensions

- Security
- Architecture
- Code quality
- General correctness and completeness

### 5) Present findings

Group by file and severity:

- 🔴 Critical
- 🟠 Major
- 🟡 Minor
- 💡 Suggestion

End with an overall recommendation: approve / request changes / approve with suggestions.

### 6) Optional posting

If requested, post selected findings back to the PR as review threads.
