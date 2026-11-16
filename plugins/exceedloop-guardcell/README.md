# ExceedLoop Guardcell

ExceedLoop Guardcell lets your coding agent run security scans and act on the results. The agent can request a scan of a repository, container image or infrastructure-as-code, read the findings with their severity and location, fix the code, and report the fix back so Guardcell can confirm it. Finding text is treated as untrusted input, and confirming a finding never hides it.

## What it adds

- The remote MCP server `https://api.guardcell.dev/api/mcp` (streamable HTTP).
- Sign-in with your ExceedLoop account through OAuth the first time a tool is used. No API keys to paste.

## Setup

1. Install the plugin, or add the MCP server URL above as a custom connector.
2. Ask your agent something like "list my latest Guardcell scans" and sign in when the browser opens.

You need an ExceedLoop account. Learn more at https://guardcell.dev.

## Support

sales@exceedloop.ai · [Privacy policy](https://app.exceedloop.ai/legal/privacy) · [Terms](https://app.exceedloop.ai/legal/terms)
