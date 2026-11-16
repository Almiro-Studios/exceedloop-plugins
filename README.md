# ExceedLoop plugins

Plugins and MCP setup for [ExceedLoop Specs](https://app.exceedloop.ai), for Cursor, Claude Code, VS Code and any MCP client.

## Cursor

[Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=exceedloop-specs&config=eyJ1cmwiOiJodHRwczovL2FwcC5leGNlZWRsb29wLmFpL2FwaS9tY3AifQ==), or install the `exceedloop-specs` plugin from the Cursor Marketplace.

## Claude Code

```bash
/plugin marketplace add Almiro-Studios/exceedloop-plugins
/plugin install exceedloop-specs@exceedloop
```

Or without the plugin: `claude mcp add --transport http exceedloop-specs https://app.exceedloop.ai/api/mcp`

## Claude.ai, ChatGPT and other clients

Add a custom connector with the URL `https://app.exceedloop.ai/api/mcp` and sign in with your ExceedLoop account.

## VS Code

```json
{ "servers": { "exceedloop-specs": { "type": "http", "url": "https://app.exceedloop.ai/api/mcp" } } }
```

The server is also in the official MCP Registry as `ai.exceedloop/specs`.

## Support

sales@exceedloop.ai · [Privacy](https://app.exceedloop.ai/legal/privacy) · [Terms](https://app.exceedloop.ai/legal/terms)
