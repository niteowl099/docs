---
description: "Conservative, iterative, and advanced code-building strategies for Copilot and AI bots."
---

# Code-Building Strategies

## Conservative/Iterative Building

- Outline modules and pseudocode for core features before writing code.
- Implement the simplest, smallest code blocks first.
- Validate code after each block or logical structure is added.
- Add complexity incrementally, testing and validating at each step.
- For complex lines (e.g., with many paired elements), add one line at a time and validate after each.

## Binary Debugging (for persistent errors)

- If errors persist, remove half of the new code (store in a temp file) and test.
- If the error is fixed, the bug is in the removed half; otherwise, restore and remove the other half.
- Repeat recursively (halving blocks) until the buggy block is isolated.
- Restore all non-buggy code and rebuild the buggy block incrementally.

## When to Switch Strategies

- Use conservative/iterative by default.
- Switch to binary debugging if errors persist after 2–3 normal attempts.
- If both fail, consider rebuilding from scratch or escalating to a human reviewer.

## Other Useful Strategies

- Use AI-assisted code review prompts to catch subtle issues.
- Use test-driven development for critical modules.
- Document all strategy switches and rationale in the changelog.
