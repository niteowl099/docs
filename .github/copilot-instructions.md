# GitHub Copilot Instructions

## About This Project

This repository is a documentation system that serves as the single source of truth for an AI-assisted development ecosystem. The entire system is built on a set of core principles and a specific, structured approach to documentation.

## Core Principles

1.  **Johnny.Decimal Structure:** All files and directories are organized using the Johnny.Decimal system (e.g., `10-19-Architecture-and-Design`, `10.01-System-Constitution.md`). When creating new files, always follow this convention.
2.  **Documentation as Truth:** The Markdown files in this repository are the canonical source of all project knowledge. Always refer to them for context and guidance.
3.  **Subscription-First AI:** Prioritize using features included in existing subscriptions (like this Copilot integration) over pay-per-use APIs.
4.  **VS Code as the Hub:** All development and orchestration are centered within the VS Code IDE.
5.  **Atomic Commits:** All changes must be committed in small, logical, and well-documented units.

## Key Document Locations

*   **System Overview & How-To:** `00-09-System-Core-and-Meta/`
*   **High-Level Strategy & Architecture:** `10-19-Architecture-and-Design/` and `10.00-Strategy/`
*   **Implementation & Roadmap:** `20-29-MVS-Bootstrap-and-Implementation/`
*   **Agent Instructions & Prompts:** `30-39-Agent-Definitions-and-Prompts/`
*   **Research & Decision Logs:** `50-59-Research-and-Decision-Logs/`

## Common Tasks

*   **To understand the project's purpose,** refer to `10.01-System-Constitution.md`.
*   **For documentation standards (arc42, C4, Zettelkasten),** consult `10.02-Documentation-Standards.md`.
*   **To create a new component,** follow the instructions in `instructions/create-new-component.md`.
*   **To ingest a Google Doc,** use the workflow defined in `instructions/ingest-gdoc-research.md`.

Your primary goal is to assist in maintaining and expanding this documentation system while strictly adhering to its established principles and structure. Always reference the existing documents to ensure your responses are contextually accurate.
