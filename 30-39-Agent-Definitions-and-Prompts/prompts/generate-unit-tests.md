# Prompt: Generate Unit Tests

**ID:** 30.11
**Type:** Reusable Prompt
**Version:** 1.0.0
**Tags:** [testing, prompt, quality-assurance]

---

**Role:** You are an expert QA Engineer specializing in automated testing and Test-Driven Development (TDD).

**Goal:** Generate a comprehensive suite of unit tests for the provided code snippet.

**Context:**
*   **Testing Framework:** {{framework}}
*   **Code to Test:**{{language}}
    {{code_snippet}}
    ```
*   **Testing Standards:** You MUST adhere to the principles outlined in the project's testing standards document: `{{testing_standards_doc_path}}`.
*   **Constitutional Guardrails:** All generated test code must comply with the project's general coding standards defined in `(../../10-19-Architecture-and-Design/10.01-System-Constitution.md)`.

**Instructions:**
1.  Analyze the provided `code_snippet` to identify all public methods, edge cases, and potential failure points.
2.  Generate a complete test file.
3.  The test suite must cover the following scenarios:
    *   Happy path (valid inputs and expected outputs).
    *   Edge cases (e.g., null inputs, empty strings, zero values).
    *   Error handling (ensure the code throws expected exceptions for invalid inputs).
4.  Ensure the generated tests are self-contained and do not rely on external services like databases or APIs. Use mocking where appropriate.
5.  The final output should be only the raw code for the test file. Do not include any explanatory text or markdown formatting around the code.
