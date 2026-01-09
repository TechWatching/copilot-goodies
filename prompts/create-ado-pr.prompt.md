---
description: Create a pull request on Azure DevOps for the current branch to main
name: create-pr
argument-hint: "[target branch] (defaults to main)"
agent: agent
tools:
  - gitkraken/git_branch
  - gitkraken/git_log_or_diff
  - gitkraken/git_push
  - microsoft/azure-devops-mcp/repo_create_pull_request
  - microsoft/azure-devops-mcp/repo_get_pull_request_by_id
---

# Create Pull Request

Create a pull request for the current branch in workspace `${workspaceFolder}`.

- **Target branch:** `${input:targetBranch:main}`
- **Repository ID:** `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`
- **PR URL format:** `https://dev.azure.com/<organization>/<project>/_git/<repo>/pullrequest/<pullRequestId>`

## Instructions

1. **Get branch info:** Use #tool:gitkraken/git_branch to get the current branch name
2. **Push to remote:** Use #tool:gitkraken/git_push to ensure the branch is pushed
3. **Get commit history:** Use #tool:gitkraken/git_log_or_diff to analyze commits and extract:
   - Work item number (from commit messages like `#73602`)
   - Change type: `feat`, `fix`, `docs`, `refactor`, `chore`, etc.
   - Change scope: `api`, `docs`, `data`, `config`, etc.
4. **Create PR:** Use #tool:microsoft/azure-devops-mcp/repo_create_pull_request with:
   - `sourceRefName`: `refs/heads/<current-branch>`
   - `targetRefName`: `refs/heads/${input:targetBranch:main}`
   - `workItems`: extracted work item number
   - Title format: `#<ticket> <type>(<scope>): <description>`
   - Description format: see example below
5. **Return result:** Provide the PR URL

## PR Description Format

```markdown
## Summary

Brief description of what this PR accomplishes.

## Changes

- Change 1
- Change 2

## Related Work Items

- #<work-item-id>
```

## Example Output

**Title:** `#12345 feat(api): add new authentication endpoint`

**PR URL:** `https://dev.azure.com/awesome-org/awesomeproject/_git/app1/pullrequest/12345`