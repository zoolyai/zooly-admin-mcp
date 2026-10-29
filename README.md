# Zooly Admin MCP

Claude Code plugin that connects to the Zooly Admin MCP. Only Zooly admins can sign in.

## Install

```bash
claude plugin marketplace add zoolyai/zooly-admin-mcp
claude plugin install zooly-admin@zooly
```

Then start Claude Code, type `/mcp`, pick **zooly-admin** and choose **Authenticate**. Sign in with your Zooly admin account and press **Allow**.

Check it works by asking: `List the recent Zooly roster crawls.`

## What you can do

Crawl talent agency websites, build roster import tables, and set up and run outreach missions. The server also offers two prompts: `process_roster` and `send_leads`.

Full guide and example questions: https://docs.zooly.ai/docs/admin/admin-mcp

## Other servers (dev, local)

The plugin always connects to `https://app.zooly.ai/api/admin-mcp`. To use another Zooly server, skip the plugin and add the server by hand:

```bash
claude mcp add --transport http zooly-admin http://localhost:3004/api/admin-mcp
```
