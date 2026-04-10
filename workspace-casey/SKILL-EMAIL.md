# SKILL-EMAIL.md — Gmail Operations

Use this skill for all email-related tasks. Casey uses the `gmail` MCP server connected to azlan@gaiada.com.

## Available Operations

- **Search emails** — Find emails by sender, subject, date, labels
- **Read emails** — Get full email content and metadata
- **List emails** — Browse inbox, sent, or any label
- **Check for new mail** — Count recent incoming or sent messages

## Common Search Queries

### Count incoming emails for a date
Search query: `after:YYYY/MM/DD is:inbox`

### Count sent emails for a date
Search query: `after:YYYY/MM/DD in:sent`

### Search by sender
Search query: `from:sender@example.com`

### Search by subject
Search query: `subject:keyword`

### Search with multiple criteria
Search query: `from:sender@example.com after:2026/01/01 has:attachment`

### Unread emails
Search query: `is:unread is:inbox`

## Workflow

1. Use `gmail` MCP tools to search or list emails matching the request.
2. For summaries: read the email content and present a concise summary.
3. For attachments: note which emails have attachments, then use SKILL-DRIVE.md to handle file operations if needed.
4. For long threads: summarize the thread chronologically, highlighting decisions and action items.

## Response Format

When reporting on emails, include:
- Sender name and address
- Date/time
- Subject line
- Brief content summary (1-2 sentences)
- Whether attachments are present

When counting emails, report the count and date range clearly.
