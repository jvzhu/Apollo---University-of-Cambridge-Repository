# Contributing to the Apollo Repository

Thank you for your interest in contributing to the Apollo project, a research collaboration with the University of Cambridge. This document describes how to contribute and the workflow we follow.

## Code of Conduct

All contributors are expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before participating.

## Ways to Contribute

- **Data collection** — gathering and organizing data from approved sources
- **Documentation** — improving research notes, guides, and repository docs
- **Bug reports** — reporting problems with data, documentation, or automation
- **Feature requests** — suggesting improvements to the repository or workflows

## Getting Started

1. **Fork** the repository (external contributors) or create a branch (collaborators)
2. **Clone** your fork or the repository locally:
   ```bash
   git clone https://github.com/jvzhu/Apollo---University-of-Cambridge-Repository.git
   ```
3. Review the [README](README.md), [Project Management Guide](PROJECT_MANAGEMENT.md), and open issues on the [Data Gathering project board](https://github.com/users/jvzhu/projects/3)

## Contribution Workflow

### 1. Find or Create an Issue

- Check existing issues to avoid duplicates
- Create a new issue using the appropriate template:
  - **Bug Report** — for bugs or problems
  - **Feature Request** — for new features or improvements
  - **Data Collection Task** — for data gathering activities
- Wait for the issue to be triaged or assigned before starting significant work

### 2. Create a Branch

Create a branch from `main` with a descriptive name:

```bash
git checkout -b <type>/<short-description>
```

Suggested branch prefixes:

| Prefix  | Purpose                          |
| ------- | -------------------------------- |
| `data/` | Data collection or updates       |
| `docs/` | Documentation changes            |
| `fix/`  | Bug fixes                        |
| `feat/` | New features or workflow changes |

### 3. Make Your Changes

- Keep changes focused — one issue per branch/pull request
- Follow the existing structure and conventions of the repository
- For data contributions:
  - Include full citations and proper attribution for all sources
  - Verify data completeness and accuracy
  - Add sources to `data/sources.md` where applicable
  - Document metadata and file formats
- For documentation, use clear Markdown formatting consistent with existing files

### 4. Commit Your Changes

Write clear, descriptive commit messages:

```
Add census data from UK Office for National Statistics

- Include 2021 population dataset
- Add citation to data/sources.md
```

Guidelines:
- Use the imperative mood in the subject line ("Add", "Fix", "Update")
- Keep the subject line under 72 characters
- Reference related issues in the body (e.g., `Refs #12`)

### 5. Open a Pull Request

1. Push your branch and open a pull request against `main`
2. Fill out the [pull request template](.github/PULL_REQUEST_TEMPLATE.md)
3. Link the related issue using closing keywords (e.g., `Closes #12`)
4. Ensure all automated checks pass

### 6. Review Process

- A maintainer will review your pull request
- Address review feedback by pushing additional commits to your branch
- Once approved, a maintainer will merge your pull request
- The linked issue moves through the project board (Backlog → In Progress → Review → Done); see the [Project Management Guide](PROJECT_MANAGEMENT.md) for details

## Data Quality Standards

All data contributions must meet the quality checklist:

- [ ] Data completeness verified
- [ ] Data accuracy confirmed
- [ ] Proper attribution/citation included
- [ ] File format standardized
- [ ] Metadata documented

## Reporting Security Issues

Please do not report security vulnerabilities through public issues. See our [Security Policy](SECURITY.md) for how to report them responsibly.

## Questions?

If you have questions or suggestions, please open an issue in this repository.

Thank you for contributing!
