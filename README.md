# ExceedLoop plugins

Plugins and MCP setup for ExceedLoop products, for Cursor, Claude Code, VS Code and any MCP client. All servers are remote (streamable HTTP) and sign in with your ExceedLoop account through OAuth.

| Product | What it does | MCP URL | Cursor |
|---|---|---|---|
| [ExceedLoop Specs](plugins/exceedloop-specs) | Plans, solution docs, ADRs, UX docs, tasks, rules and skills. | `https://app.exceedloop.ai/api/mcp` | [Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=exceedloop-specs&config=eyJ1cmwiOiJodHRwczovL2FwcC5leGNlZWRsb29wLmFpL2FwaS9tY3AifQ==) |
| [ExceedLoop Sketchpad](plugins/exceedloop-sketchpad) | Design canvas: pages, components, PNG renders, code export. | `https://sketchpad.exceedloop.ai/mcp` | [Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=exceedloop-sketchpad&config=eyJ1cmwiOiJodHRwczovL3NrZXRjaHBhZC5leGNlZWRsb29wLmFpL21jcCJ9) |
| [ExceedLoop Guardcell](plugins/exceedloop-guardcell) | Security scans for code, containers and IaC; findings and fixes. | `https://api.guardcell.dev/api/mcp` | [Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=exceedloop-guardcell&config=eyJ1cmwiOiJodHRwczovL2FwaS5ndWFyZGNlbGwuZGV2L2FwaS9tY3AifQ==) |

## Claude Code

```bash
/plugin marketplace add Almiro-Studios/exceedloop-plugins
/plugin install exceedloop-specs@exceedloop
/plugin install exceedloop-sketchpad@exceedloop
/plugin install exceedloop-guardcell@exceedloop
```

Or without plugins:

```bash
claude mcp add --transport http exceedloop-specs https://app.exceedloop.ai/api/mcp
claude mcp add --transport http exceedloop-sketchpad https://sketchpad.exceedloop.ai/mcp
claude mcp add --transport http exceedloop-guardcell https://api.guardcell.dev/api/mcp
```

## Claude.ai, ChatGPT and other clients

Add a custom connector with the MCP URL from the table and sign in with your ExceedLoop account.

## VS Code

```json
{
  "servers": {
    "exceedloop-specs": { "type": "http", "url": "https://app.exceedloop.ai/api/mcp" },
    "exceedloop-sketchpad": { "type": "http", "url": "https://sketchpad.exceedloop.ai/mcp" },
    "exceedloop-guardcell": { "type": "http", "url": "https://api.guardcell.dev/api/mcp" }
  }
}
```

All three servers are in the official MCP Registry as `ai.exceedloop/specs`, `ai.exceedloop/sketchpad` and `ai.exceedloop/guardcell`.

## Support

sales@exceedloop.ai · [Privacy](https://app.exceedloop.ai/legal/privacy) · [Terms](https://app.exceedloop.ai/legal/terms)
