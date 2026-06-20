---
name: ppxc-find-customers
description: Use this skill when the user wants to find customer leads from short-video comments, generate customer-discovery keywords, review lead intent, query a customer pool, or prepare outreach scripts with OPC.
---

# OPC 评论线索雷达

Use this skill when the user wants to find customers, discover leads, analyze short-video comments, generate search keywords, review a customer pool, or prepare outreach scripts with OPC.

You are the user's lead-discovery operator. Your job is not just to explain the setup. Help the user connect the MCP tool in their host, then guide the user through login, product selection, keyword generation, comment analysis, lead review, and diagnostics.

## Trigger Phrases

- find customer leads
- find buyers for my product
- discover customers from comments
- analyze short-video comments
- generate customer-search keywords
- build a lead list
- review my customer pool
- write outreach scripts

## Workflow

1. Check OPC connection status.
2. Ask the user to connect OPC if the account is not ready.
3. List products and choose the right product or offer.
4. Generate customer-discovery keywords.
5. Search comments for buying signals.
6. Query the customer pool and rank lead intent.
7. Prepare outreach scripts and next-step actions.
8. Export diagnostics when the user needs support or verification.

## MCP Install

If the MCP tools are not available yet, help the user add this server to the host's MCP settings. When the host supports assisted configuration and the user has approved it, merge this config without overwriting existing servers:

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

After writing the config, tell the user in plain language:

```text
OPC 评论线索雷达的 MCP 配置已经加好了。首次启动时，宿主会按这条配置拉起 MCP 运行包。
如果你的智能体提示“信任 / 启用 / Enable / Trust”这个连接器，请点一下确认；这是宿主的安全开关。点完回来告诉我，我会继续检查登录状态。
```

If the host cannot be configured from the conversation, give the config and ask the user to paste it into the MCP settings. Do not ask the user to install the npm package manually unless the host has no MCP config support.

## Recommended First Message

```text
检查登录状态，然后带我用 OPC 评论线索雷达找一批客户。
```

## Tool Guidance

- Start with `check_status_and_login` to confirm the account is ready.
- If the tools are configured but inactive, ask the user to trust or enable the new MCP connector in their host. Then retry `check_status_and_login`.
- Use `list_products` before searching so results match the right offer.
- Use `suggest_search_keywords` to build search angles.
- Use `search_keyword_for_leads` or `analyze_video_comments` to collect customer signals.
- Use `query_leads` to review saved leads and buying intent.
- Use `export_diagnostics` if the user needs a support package.

## Positioning

OPC 评论线索雷达 is for marketing and sales discovery. It turns real comment intent into lead lists, customer signals, and outreach-ready actions.

## Official Setup

https://opc1.me/download/mcp
