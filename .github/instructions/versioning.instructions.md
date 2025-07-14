---
description: "Versioning, atomic commits, and git workflow best practices for Copilot and AI bots."
---

# Versioning and Git Workflow

## Atomic Commits

- Each commit should represent a single, logical change.
- Reference the relevant instruction or prompt file in the commit message.
- Use descriptive, meaningful commit messages.

## Branching

- Create a new branch for each significant feature, fix, or documentation update.
- Close or merge previous branches if the focus of work changes.
- Keep branches focused and short-lived to minimize merge conflicts.

## Versioning

- Use semantic versioning (e.g., 1.2.3) for significant updates.
- Tag each atomic commit or merge with a version number if it represents a release or milestone.
- Decide on system-wide or per-repo versioning based on project needs; document the approach in the repo README.

## Best Practices

- Always check for open bugs, errors, or challenges before merging.
- Document all versioning and branching decisions in the changelog.
- Automate version/tag assignment where possible.
