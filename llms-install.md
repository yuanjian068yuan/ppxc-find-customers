# OPC 评论线索雷达 Agent Setup Guide

Use this guide when an agent or MCP host needs to enable OPC 评论线索雷达.

## What This Is

- Skill is the business workflow: it tells the agent how to check login, choose a product, generate keywords, find customer leads, query the customer pool, and prepare outreach scripts.
- MCP is the runtime tool: it gives the host the actual tools for OPC login, product selection, keyword generation, comment analysis, customer-pool query, and diagnostics.
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
2. Ask the agent to check OPC login status.
3. If OPC is not connected, follow the login instructions returned by the MCP.
4. Choose a product or offer before searching.
5. Generate customer-discovery keywords.
6. Search short-video comments for customer intent.
7. Review the customer pool and prepare outreach scripts.

## Useful Starting Prompt

```text
Find customer leads for my product.
```

## Search Intent Coverage

Use this skill for 找客户、销售线索、评论分析、关键词、客户池、跟进话术、小红书获客、抖音获客、快手获客、lead generation from comments, customer discovery skill, and short video lead generation.

## Support

Official setup page: https://opc1.me/download/mcp
Official facts page: https://opc1.me/facts
