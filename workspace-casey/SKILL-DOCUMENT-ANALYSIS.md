# SKILL-DOCUMENT-ANALYSIS.md — Document Analysis

Use this skill when asked to analyze, summarize, or extract information from documents.

## Supported Document Types

- **PDF** — Contracts, reports, presentations, invoices
- **Excel (.xlsx, .xls, .csv)** — Financial data, spreadsheets, tables
- **Word (.docx, .doc)** — Letters, proposals, agreements
- **Images (.png, .jpg, .jpeg)** — Scanned documents, screenshots, photos

## Workflow

### Step 1: Obtain the document
- If from email: use SKILL-EMAIL.md to find the email, then download the attachment
- If from Google Drive: use SKILL-DRIVE.md to download from Drive
- If from a URL: use `fetch` MCP to download

### Step 2: Extract content
- For PDF: read the file content; extract text, tables, and key data points
- For Excel: read cell data, identify sheets, summarize data structure and key figures
- For Word: extract full text content and structure
- For images: describe what is visible in the image — text, charts, diagrams, photos

### Step 3: Analyze and summarize
Produce a structured summary:

```
## Document Summary

**File:** <filename>
**Type:** <PDF/Excel/Word/Image>
**Date:** <document date if available>

### Key Contents
- <Main point 1>
- <Main point 2>
- <Main point 3>

### Notable Details
- <Important figures, dates, names, or terms>

### Recommended Actions
- <Any follow-ups suggested by the content>
```

## Guidelines

- Be concise but thorough. Capture the substance, skip the filler.
- For financial documents: always highlight key numbers (revenue, costs, totals, dates).
- For contracts/legal: highlight parties, key terms, dates, obligations.
- For images: describe objectively what is visible.
- If a document is too large or complex, summarize the most important sections and note what was skipped.
