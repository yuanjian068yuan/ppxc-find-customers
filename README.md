# PPXC Find Customers

Turn short-video comments into customer leads, keyword ideas, and outreach scripts.

PPXC Find Customers is a marketing MCP for founders, marketers, sales operators, and creators who want to find buyers from real public comment signals. It helps your MCP host move from product selection to lead discovery, lead review, and outreach preparation.

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

Official setup page: https://opc1.me/download/mcp

## What It Does

- Checks whether PPXC is connected and ready.
- Selects the right product or offer before searching.
- Suggests customer-discovery keywords.
- Searches short-video comments for buying signals.
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
Find customer leads for my product.
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

Use PPXC Find Customers only with public comment data and data you are authorized to process. Do not paste passwords, payment data, recovery codes, API keys, private customer records, or other secrets into prompts.

## Support

- Setup: https://opc1.me/download/mcp
- Contact: yuanjian068@gmail.com
