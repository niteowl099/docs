---
description: "First step in the development lifecycle for all Copilot and AI-assisted development."
---

# Directive Handling Workflow

If the user's intent is a directive (feature, bug, goal, etc.), follow this workflow:

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

# After User Confirmation

Once the user confirms the plan:

- The AI should minimize further user interaction by collecting all steps that might need approval and otherwise proceed autonomously.
- The AI should use simple tests and incremental validation to ensure reliable, error-free code generation.
- If persistent or chained errors/bugs occur, the AI should switch to a more conservative or advanced debugging strategy as described in [debugging.instructions.md](./debugging.instructions.md).
- If everything is implemented as expected, the AI should ask if the user wants to commit, push, or move to the next phase.

# Strategy Guidance

Refer to the following instruction files for detailed strategies:

- [code-building.instructions.md](./code-building.instructions.md): Conservative, iterative, and advanced code-building strategies.
- [debugging.instructions.md](./debugging.instructions.md): Binary debugging, error isolation, and other advanced debugging strategies.
- [versioning.instructions.md](./versioning.instructions.md): Versioning, atomic commits, and git workflow best practices.

> **Note:** The AI should always try to optimize for efficient, reliable code creation and minimal user interaction, but must switch strategies if errors persist.
