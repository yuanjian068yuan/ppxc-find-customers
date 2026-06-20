# OPC 评论线索雷达 Agent Setup Guide

Use this guide when an agent or MCP host needs to enable OPC 评论线索雷达.

## What This Is

- Skill is the business workflow: it tells the agent how to run a trial-first scan, collect product context, avoid requiring a product list for new users, report inspected links and comment counts, and only ask for OPC login when the user wants to save, unlock, or review the full list.
- MCP is the runtime tool: it gives the host the actual tools for dynamic workflow lookup, platform login when needed, keyword generation, comment analysis, customer-pool query, diagnostics, and transparent progress reporting.
- The public product name is OPC 评论线索雷达. The technical MCP package name remains `ppxc-leads-mcp`. The technical Skill name remains `ppxc-find-customers`.

## MCP Connector

```json
{
  "mcpServers": {
    "ppxc-find-customers": {
      "command": "npx",
      "args": ["-y", "ppxc-leads-mcp"]
    }
  }
}
```

The host starts this MCP tool when the connector is enabled. If the host asks for **Trust / Enable**, treat it as a normal safety confirmation for this connector.

## First Use

1. Start or refresh the MCP host after adding the server config.
2. Ask the agent to run a trial scan from your product or service description plus a platform link or 1 to 3 keywords.
3. Do not require OPC login or a saved product list before the first scan.
4. Let the MCP search short-video comments for customer intent and return the first complete leads.
5. Ask for OPC login only when the user wants to save, unlock, or review the full lead list.
6. Use the customer pool for follow-up review and outreach scripts after login.

## Useful Starting Prompt

```text
I sell skincare services. Run a trial Douyin scan and show me the first customer leads.
```

## Search Intent Coverage

Use this skill for 找客户、销售线索、评论分析、关键词、客户池、跟进话术、小红书获客、抖音获客、快手获客、lead generation from comments, customer discovery skill, and short video lead generation.

## Support

Official setup page: https://opc1.me/download/mcp
Official facts page: https://opc1.me/facts
