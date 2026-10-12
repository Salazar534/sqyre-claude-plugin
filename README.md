# Sqyre for Claude

Public Claude plugin for a Sqyre home-service company. It connects Claude to the Sqyre MCP server and teaches it how to use the books, the schedule, and the client record.

Production server: `https://api.sqyre.ai/api/v1/mcp`  
Sign-in: `https://api.sqyre.ai/oauth/v1`

Claude asks the person to sign in the first time. This repository does not contain API keys or customer data.

## What is in the package

- `.claude-plugin/plugin.json` is the manifest. The plugin name is `sqyre` and the version is `1.0.0`.
- `skills/` holds one skill per area of the business.
- `.mcp.json` points Claude at the Sqyre MCP server.

## Try it locally

```bash
claude --plugin-dir /path/to/sqyre-claude-plugin
claude plugin validate /path/to/sqyre-claude-plugin
```

## Install from GitHub

In Claude Code:

```text
/plugin marketplace add Salazar534/sqyre-claude-plugin
/plugin install sqyre@sqyre-claude-plugin
```

Or pass this repository URL in the Anthropic plugin submission form: https://github.com/Salazar534/sqyre-claude-plugin
