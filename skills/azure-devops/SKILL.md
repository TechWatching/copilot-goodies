---
name: azure-devops
description: Provides reusable Azure DevOps workspace configuration. Use when working with work items, pull requests, pipelines, repositories, iterations, or any Azure DevOps operation in this workspace.
argument-hint: "[work item type] [action to perform]"
---

# Azure DevOps Configuration

## Organization & Project

- **Organization**: `<ADO_ORG>`
- **Project Name**: `<ADO_PROJECT_NAME>`
- **Project ID**: `<ADO_PROJECT_ID>`
- **Organization URL**: `https://dev.azure.com/<ADO_ORG>`
- **Project URL**: `https://dev.azure.com/<ADO_ORG>/<ADO_PROJECT_URL_SEGMENT>`

## Work Item Types

- Epic
- Feature
- User Story
- Bug
- Task

## Usage Guidelines

1. Always pass `project: <ADO_PROJECT_NAME>`.
2. Use the correct repository ID for branch/commit/PR artifact linking.
3. Output work-item links as:  
   `https://dev.azure.com/<ADO_ORG>/<ADO_PROJECT_URL_SEGMENT>/_workitems/edit/{workItemId}`
4. Use Markdown format for long text fields.
5. Read the current work item before update to avoid overwriting concurrent changes.
6. Follow existing tags/naming/field usage conventions from current project data.

## Optional per-workspace extensions

Add or remove sections depending on your environment:
- Iteration/team defaults
- Deployment-specific required fields
- PR/repo mapping conventions
- Pipeline/release linking conventions