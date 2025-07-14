# How to Ingest Google Doc Research Reports

This document outlines the standard procedure for ingesting research and reports from Google Docs into this documentation system.

## Workflow

1.  **Obtain the Google Doc URL:** Start with the full URL of the Google Doc containing the research report.

2.  **Initiate the Ingestion:** Instruct the agent to begin the ingestion process by providing the URL.

3.  **Agent Processing:** The agent will perform the following steps:
    *   Use the `web_fetch` tool to access and extract the full content of the Google Doc.
    *   Determine the correct filename and path within the `50-59-Research-and-Decision-Logs/` directory. The filename should be descriptive (e.g., `50.XX-Summary-of-New-Technology.md`).
    *   Create a new markdown file.
    *   Add a metadata block (YAML front matter) to the top of the file with the following format:
        ```yaml
        ---
        source_gdoc_url: '[URL]'
        ingestion_date: 'YYYY-MM-DD'
        status: 'draft'
        version: '1.0'
        tags: ['research', 'ingestion', 'topic']
        ---
        ```
    *   Paste the full content extracted from the Google Doc into the new file below the metadata block.

4.  **Commit the Changes:** Once the file is created, the agent will perform an atomic commit with a descriptive message, such as `docs: Ingest research report on [Topic]`.
