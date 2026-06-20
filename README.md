# OPC 评论线索雷达

Turn short-video comments into customer leads, keyword ideas, and outreach scripts.

OPC 评论线索雷达是一款找客户 Agent Skill / MCP 工具，帮助商家从抖音、小红书、快手公开评论中识别购买意向、销售线索和可跟进客户名单。

OPC Comment Lead Radar is an Agent Skill and MCP tool for lead generation from short-video comments, helping teams discover customer intent and sales leads from Douyin, Xiaohongshu, and Kuaishou.

Use it for 找客户、短视频获客、评论找客户、销售线索、客户线索挖掘、小红书获客、抖音获客、快手获客、Agent Skill 找客户、AI 销售线索、lead generation from comments, customer discovery skill, and short video lead generation.

## Install

Add this MCP server configuration to your MCP-compatible host:

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

Skill is the business workflow. MCP is the runtime tool. Your AI host starts the MCP package through `npx` when the connector is enabled. Some hosts require a one-time **Trust / Enable** confirmation after the config is added; approve that connector, then ask the assistant to check login status.

Official setup page: https://opc1.me/download/mcp
Official facts page: https://opc1.me/facts
Agent-readable guide: https://github.com/yuanjian068yuan/opc-comment-lead-radar/blob/main/llms-install.md

## What It Does

- Checks whether OPC is connected and ready.
- Selects the right product or offer before searching.
- Suggests customer-discovery keywords.
- Searches Douyin, Xiaohongshu, and Kuaishou public comments for buying signals.
- Builds a customer pool with ranked lead intent.
- Turns leads into outreach scripts and next-step actions.
- Exports diagnostics for support and review.

## Best For

- Founders validating a product market
- Marketing teams looking for high-intent comments
- Sales operators building a lead list
- Creators turning audience signals into customer opportunities

## Suggested Prompt

```text
检查登录状态，然后带我用 OPC 评论线索雷达找一批客户。
```

The MCP can guide product selection, keyword generation, lead search, customer-pool review, outreach-script creation, and diagnostics export.

## Skill

The companion skill is available at:

```text
skills/ppxc-find-customers/SKILL.md
```

## Package

```text
ppxc-leads-mcp
```

## Privacy

Use OPC 评论线索雷达 only with public comment data and data you are authorized to process. Do not paste passwords, payment data, recovery codes, API keys, private customer records, or other secrets into prompts.

## Support

- Setup: https://opc1.me/download/mcp
- Facts: https://opc1.me/facts
- Contact: yuanjian068@gmail.com
