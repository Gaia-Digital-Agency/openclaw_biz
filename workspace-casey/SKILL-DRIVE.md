# SKILL-DRIVE.md — Google Drive Operations

Use this skill for all Google Drive file management tasks. Casey uses the `google-drive` MCP server connected to the azlan@gaiada.com Google account.

## Available Operations

- **List files** — Browse files and folders in Google Drive
- **Upload files** — Upload local files to Google Drive
- **Download files** — Download files from Google Drive to local storage
- **Search files** — Find files by name, type, or content
- **Create folders** — Organize files in Drive

## Common Workflows

### Download attachment from email and store in Drive
1. Use SKILL-EMAIL.md to find and read the email with the attachment.
2. Download the attachment using gmail MCP tools.
3. Upload the file to the appropriate Google Drive folder using google-drive MCP tools.
4. Confirm the upload with file name and Drive location.

### List files in a Drive folder
1. Use google-drive MCP tools to list contents of the specified folder.
2. Present the file list with names, types, and modification dates.

### Download a file from Drive for analysis
1. Use google-drive MCP tools to download the file.
2. Save to the local workspace or temp directory.
3. Hand off to SKILL-DOCUMENT-ANALYSIS.md if analysis is requested.

## Response Format

When reporting file operations:
- File name and type
- Source and destination paths
- Confirmation of success or error details
