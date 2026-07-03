# GitHub Actions Automation Guide

## Overview
This document describes the automated workflows configured for your repositories.

## Available Workflows

### 1. Issue Auto-Management
**File:** `issue-automation.yml`
- Automatically adds new issues to the Data Gathering project board
- Auto-labels issues based on keywords in title/description
- Auto-assigns issues to team members based on labels

### 2. Pull Request Workflows
**File:** `pr-automation.yml`
- Automatically links PRs to related issues
- Auto-requests reviewers based on file changes
- Runs automated checks and tests

### 3. Project Board Automation
**File:** `project-board-automation.yml`
- Moves issues through workflow stages automatically
- Archives completed tasks after 30 days
- Closes stale issues (60+ days inactive)

### 4. Data Collection Validation
**File:** `data-collection-validation.yml`
- Validates data collection PRs
- Checks for required metadata and documentation
- Auto-generates collection reports

### 5. Changelog & Release Management
**File:** `changelog-release.yml`
- Auto-generates CHANGELOG.md from commits
- Creates releases automatically
- Updates documentation on release

### 6. Project Board Setup
**File:** `setup-project-board.yml`
- Creates the **Data Gathering** project board (if it doesn't already exist)
- Configures the Status columns: Backlog, In Progress, Review, Done
- Adds all existing open issues to the board
- Triggered manually from the **Actions** tab (workflow_dispatch)
- Requires a `PROJECT_TOKEN` repository secret: a personal access token with the `project` scope (the default `GITHUB_TOKEN` cannot create user-owned projects)

### 7. Documentation Updates
**File:** `docs-update.yml`
- Keeps README.md current
- Updates PROJECT_MANAGEMENT.md with metrics
- Maintains issue templates

## Running Workflows

### Manual Trigger
Go to **Actions** tab and select a workflow, then click **Run workflow**

### Automatic Triggers
- **Issues:** When issue is created or reopened
- **PRs:** When PR is created or reopened
- **Scheduled:** Weekly checks for stale content
- **Push:** On commits to main branch

## Disabling Workflows
Edit the workflow file and remove the trigger condition, or disable in Actions settings.

## Troubleshooting
If workflows fail:
1. Check the **Actions** tab for error logs
2. Verify repository secrets are configured
3. Ensure branch protections allow automated commits

---
**Last Updated:** 2026-06-21
