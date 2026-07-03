# Project Management Guide

## Overview
This document outlines the project management workflow for the Apollo Repository collaboration with the University of Cambridge.

## Project Board Structure

### Board: Data Gathering
**URL:** https://github.com/users/jvzhu/projects/3

#### Columns:
1. **Backlog** - New issues ready for work
2. **In Progress** - Currently being worked on
3. **Review** - Awaiting review or feedback
4. **Done** - Completed and merged

#### Board Setup
The board can be created (or re-synced) automatically by running the
**Setup Project Board** workflow (`.github/workflows/setup-project-board.yml`)
from the **Actions** tab. It creates the board, configures the columns above,
and adds all existing open issues. It requires a `PROJECT_TOKEN` repository
secret containing a personal access token with the `project` scope.

## Workflow

### Creating an Issue
1. Click **New issue** in the repository
2. Choose a template:
   - **Bug Report** - For bugs or issues
   - **Feature Request** - For new features
   - **Data Collection Task** - For data gathering activities
3. Fill out all required fields
4. Assign to yourself or team member
5. Add appropriate labels
6. Issue automatically added to project board (Backlog)

### Moving Issues Through Workflow

#### Backlog → In Progress
- Assign the issue to yourself
- Add comment: "Starting work on this"
- Project workflow automatically updates status

#### In Progress → Review
- Create a pull request linking to the issue
- Add comment with PR link
- Request review from team members

#### Review → Done
- Pull request approved
- Merge to main branch
- Close issue
- Issue automatically moves to Done

## Labels

### By Type
- `bug` - Bug reports
- `enhancement` - Feature requests
- `documentation` - Documentation updates
- `data collection` - Data gathering tasks

### By Priority
- `critical` - Blocks other work
- `high` - Important
- `medium` - Standard priority
- `low` - Nice to have

### By Status
- `in-progress` - Currently being worked on
- `blocked` - Blocked by another issue
- `help-wanted` - Seeking assistance
- `good-first-issue` - Good for new contributors

## Milestones

- **v0.1** - Initial setup and data collection
- **v0.2** - Analysis and categorization
- **v1.0** - First release

## Best Practices

1. **Keep issues focused** - One task per issue
2. **Use descriptive titles** - Clear problem statement
3. **Add labels** - Categorize for filtering
4. **Link related issues** - Reference connections
5. **Update status regularly** - Keep project board current
6. **Close completed issues** - Mark as done when finished
7. **Review before merging** - Ensure quality

## Automation

The repository includes automated workflows that:
- Automatically add new issues to the project board
- Set default status to "Backlog" for new issues
- Assign issues to the Backlog column

## Team Guidelines

### Issue Assignment
- Issues are assigned to `jvzhu` by default
- Team members can reassign as needed
- Each person should only have 3-5 active issues

### Review Process
1. Create pull request with detailed description
2. Link to issue(s) being addressed
3. Request review from at least one team member
4. Address feedback and make updates
5. Merge once approved

### Communication
- Use issue comments for discussion
- Tag team members with @username
- Provide context for complex issues
- Link related resources and references

## Metrics

Track progress using:
- **Issues created** - New work identified
- **Issues in progress** - Current workload
- **Issues completed** - Velocity
- **Cycle time** - Time from created to done

## Resources

- [GitHub Projects Documentation](https://docs.github.com/en/issues/planning-and-tracking-with-projects)
- [Issue Templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)
- [GitHub Actions](https://docs.github.com/en/actions)

---

**Last Updated:** 2026-06-21  
**Maintained by:** jvzhu
