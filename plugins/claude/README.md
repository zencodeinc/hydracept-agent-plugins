# Hydracept for Claude

One execution surface for text/reasoning, media, domains, DNS, and other external capabilities, with durable jobs, budgets, receipts, and BYOK.

Plugin homepage: https://hydracept.com/plugin

A Zencode product · © Zencode Consulting Inc.

Add the Hydracept marketplace, then install the namespaced plugin:

```text
/plugin marketplace add zencodeinc/hydracept-agent-plugins
/plugin install hydracept@hydracept
```

In a project checkout run `python -m hydracept init --apply --yes --json`, then reload MCP. Stdio uses `.hydracept/secrets.json`. Hosted MCP (`https://api.hydracept.com/mcp`) is for clients with no checkout.

Commands: `/hydracept-init`, `/hydracept-doctor`.

Local CLI fallback (optional): `python -m hydracept agents install --auto`.
