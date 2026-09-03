# Hydracept for Cursor

One execution surface for text/reasoning, media, domains, DNS, and other external capabilities, with durable jobs, budgets, receipts, and BYOK.

Plugin homepage: https://hydracept.com/plugin

A Zencode product · © Zencode Consulting Inc.

Install from the Cursor Marketplace, or clone `https://github.com/zencodeinc/hydracept-agent-plugins` and enable the Cursor plugin under `plugins/cursor`.

In a project checkout run `python -m hydracept init --apply --yes --json`. That writes workspace secrets and binds project MCP to stdio (`python -m hydracept mcp serve`). Reload MCP once. Do not copy the workspace key into **Plugins → Configure**.

Commands: `/hydracept-init`, `/hydracept-doctor`.

Local CLI fallback (optional): `python -m hydracept agents install --auto`.
