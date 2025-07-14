# Reusable Prompt: Ingest Google Doc

## Agent Task

You will be provided with a Google Doc URL. Your task is to ingest the content of this document into our documentation system by following these steps precisely:

1.  **Extract Content:** Use the `web_fetch` tool to extract the complete text content from the provided Google Doc URL.

2.  **Determine File Path:** The new file must be created within the `50-59-Research-and-Decision-Logs/` directory. Create a descriptive filename based on the document's content, following the `XX.YY-title.md` format.

3.  **Create Metadata:** At the very top of the new file, create a YAML front matter block with the following information:
    *   `source_gdoc_url`: The full URL of the source Google Doc.
    *   `ingestion_date`: The current date in `YYYY-MM-DD` format.
    *   `status`: Set to `draft`.
    *   `version`: Set to `1.0`.
    *   `tags`: An array of relevant tags (e.g., `['research', 'ingestion', 'topic']`).

4.  **Write the File:** Write the extracted content into the new markdown file, immediately following the YAML front matter.

5.  **Commit the File:** After creating the file, perform a `git add` and `git commit` for the new file. The commit message must be atomic and follow the convention: `docs: Ingest research report on [Topic]`.
