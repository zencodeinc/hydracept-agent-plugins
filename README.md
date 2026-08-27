# Hydracept agent plugins

Hydracept gives game teams production-ready assets through one API. Every job leaves a receipt.

A Zencode product · © Zencode Consulting Inc. · MIT License

Version `0.1.5` (marketplace `distributionVersion`, independent of the Python SDK).

This public repo is the **Cursor / Claude / MCP catalog**. Plugin homepage: [https://hydracept.com/plugin](https://hydracept.com/plugin). Cursor Marketplace review should use `.cursor-plugin/marketplace.json` and `plugins/cursor`.

## Cursor Marketplace

Plugin path: `plugins/cursor`

1. Install **Hydracept** from the Cursor Marketplace (or enable this repository as a plugin catalog).
2. In the project, run `python -m hydracept init --apply --yes --json` (CLI `0.3.0` contract). Init binds `.cursor/mcp.json` and `.mcp.json` to stdio MCP. Get a key at [hydracept.com/start](https://hydracept.com/start) or via the init browser flow. Do not paste the key into chat.
3. Reload MCP once. Do not copy the workspace key into **Plugins → Configure**. Hosted MCP at `https://api.hydracept.com/mcp` is for clients with no checkout.

Included for Cursor:

- Stdio MCP (`mcp.json`) — `python -m hydracept mcp serve`, no secrets in git
- Skills: `hydracept`, `hydracept-setup`, `hydracept-image`, `hydracept-sheet`, `hydracept-smoke`
- Commands: `/hydracept-init`, `/hydracept-doctor`
- Rule: never solicit API keys in chat; stdio after init in a repo

## Claude Code

```text
/plugin marketplace add zencodeinc/hydracept-agent-plugins
/plugin install hydracept@hydracept
```

Run `python -m hydracept init` in the repo, then reload MCP. Do not paste keys into chat.

## MCP Registry

Remote server `com.hydracept/mcp` at `https://api.hydracept.com/mcp`.

## Security

This repository contains **no API keys or tokens**. In a checkout, `python -m hydracept init` stores secrets in `.hydracept/secrets.json` (gitignored). Coding-agent MCP is stdio. Hosted MCP bearer keys are only for clients with no checkout (MCP Registry / ChatGPT).

## CLI fallback

```bash
pip install hydracept
python -m hydracept agents install --auto
```
