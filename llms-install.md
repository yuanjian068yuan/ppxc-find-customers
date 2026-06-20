# OPC 评论线索雷达 Installation Guide

Use this guide when an agent or MCP host needs to install OPC 评论线索雷达.

## MCP Server

Install through the published npm package:

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

## First Run

1. Start the MCP host after adding the server config.
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

## Support

Official setup page: https://opc1.me/download/mcp
