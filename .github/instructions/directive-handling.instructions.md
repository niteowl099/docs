---
description: "Handle user directives: feature requests, bug reports, product guidance, and development goals."
---

# Directive Handling Workflow

If the user's intent is a directive (feature, bug, goal, etc.):

1. **Extract all relevant directives and guidance from the user.**
   - Preserve all granular details and specificity in the user's prompt.
2. **Propose a detailed, phased implementation plan.**
   - Reference all relevant instruction files for each phase (e.g., code building, debugging, testing, review).
   - Outline modules, pseudocode, and core features for the current phase.
   - Suggest the most efficient and reliable code-building and debugging strategies (see [code-building.instructions.md](./code-building.instructions.md) and [debugging.instructions.md](./debugging.instructions.md)).
   - Check for any previously documented bugs, errors, or challenges that may be relevant.
3. **Describe the intended git/repo/branch/versioning plan.**
   - Indicate if a new branch should be created, if a previous branch should be closed, or if a merge/commit is needed.
   - Recommend atomic commits and versioning best practices (see [versioning.instructions.md](./versioning.instructions.md)).
4. **Present all of the above in a single turn for user review and confirmation.**
   - The user should only need to review, confirm, reject, or provide further guidance.

> **Strict adherence:** Steps 1–4 must be completed in a single AI turn unless the user instructs otherwise.
