# macci 2.7.3

A macOS notch companion: media controls, calendar, file shelf, HUD replacement,
work logbook — plus an on-screen AI assistant and pointer.

## What's new

**Bring your own AI**
- Pick your provider and API key in **Settings → AI Model**: OpenAI, Anthropic,
  xAI (Grok), Google Gemini, or the built-in default with nothing to set up.
- Model names are free-text — type whatever your key can reach.

**On-screen assistant**
- Draws **arrows, boxes and circles** to point things out and explain what's on screen.
- **Guided walk-throughs** — step-by-step arrows to the exact next control in any app.
- **Autonomous agent** — hand it a whole task; a floating card streams progress and
  **asks before anything is sent, submitted, deleted or paid**. Runs on whichever
  provider you picked.

**Logbook**
- **Connectors** (Settings → Connections): push entries and AI summaries to
  **Slack, GitHub Issues, Linear, Notion**, or a custom webhook. Jira unchanged.
- **MCP connectors** — attach Model Context Protocol servers (HTTP/SSE) and the
  agent can call their tools.
- **Skills** (Settings → Skills) — plain-language instructions for your recurring
  tasks, auto-applied by app and keyword.

## Install

Download `macci-2.7.3.dmg`, open it, drag **macci** to Applications. The build is
notarized by Apple — it opens with no Gatekeeper warning. Universal (Apple Silicon
+ Intel), macOS 14.2+.

## Verify

```
spctl -a -vvv -t open --context context:primary-signature macci-2.7.3.dmg
# → accepted · source=Notarized Developer ID · Michael Nkomo (SFTLP3DWGA)
```
