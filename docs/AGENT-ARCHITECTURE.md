# Agent Architecture

Case is a multi-agent AI system built on OpenClaw.

## Agents

| Agent | ID | Workspace |
|-------|----|-----------|
| **Case** | casey | workspace-casey |
| **Casey** | main | workspace-main |
| **Writer** | writer | workspace-writer |

## Delegation

Case (main) delegates to: writer

## Configuration

- State dir: `/opt/.openclaw-biz`
- Config: `/opt/.openclaw-biz/openclaw.json`
- Gateway port: 19189
- Model: deepseek/deepseek-chat (fallback: google/gemini-2.5-flash)

## Workspace Structure

Each agent workspace follows:

```
workspace-{agent}/
  IDENTITY.md      -- Name, role
  SOUL.md          -- Voice and output rules
  USER.md          -- Owner context
  TOOLS.md         -- Available tools
  SKILLS.md        -- Skill index
  SKILL-*.md       -- Specific workflows
```
