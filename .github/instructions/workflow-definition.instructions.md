---
description: "Defining, documenting, and following workflows and processes in the workspace."
---

# Workflow Definition and Management Instructions

## 1. Workflow Definition Intention Detection

- The AI must always check if the user's intent is to define, update, or clarify a workflow or process.
- If workflow definition is detected, route to this instruction set and follow all steps strictly.

## 2. Workflow Definition Procedure

1. **Extract Workflow Purpose and Scope**
   - Ask the user to clearly state the purpose, scope, and context of the workflow.
   - Document the workflow's intended outcome and boundaries.
2. **Identify and List All Distinct Steps**
   - Break down the workflow into discrete, clearly separated steps.
   - Each step must have a single, well-defined function or behavior.
   - Use numbered lists for sequential steps; use sub-lists for conditional or parallel branches.
3. **Describe Inputs, Outputs, and Preconditions**
   - For each step, specify required inputs, expected outputs, and any preconditions or dependencies.
4. **Document Roles and Responsibilities**
   - Identify who (AI, user, team, tool) is responsible for each step.
5. **Reference Related Instruction Files and Documentation**
   - Link to any relevant instruction files, best practices, or external documentation for each step.
6. **Review and Confirm Workflow**
   - Present the full workflow to the user for review and explicit confirmation before implementation.
7. **Version and Document the Workflow**
   - Store the workflow in a dedicated instruction or documentation file.
   - Update the changelog and cross-link from central workflow/process documentation.

## 3. Workflow Execution Procedure

- When following a workflow, the AI must:
  1. Strictly adhere to the documented steps in order.
  2. Clearly indicate the current step and expected outcome at each stage.
  3. Pause for user input or confirmation at designated steps.
  4. Document all deviations, exceptions, or changes, and update the workflow documentation as needed.

## 4. Workflow Documentation and Maintenance

- All workflows must be versioned, cross-referenced, and discoverable from central documentation.
- Any changes to workflows must follow the documentation-first workflow and be reviewed/confirmed by the user.
- New or updated workflows must include:
  - Title, description, and scope
  - Step-by-step breakdown
  - Roles and responsibilities
  - References to related instructions
  - Version history and changelog entries

> **Strict adherence:** All workflow definition and execution must follow these procedures. No workflow or process should be implemented or changed without following this instruction set.
