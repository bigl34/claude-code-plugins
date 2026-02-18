<!-- AUTO-GENERATED README — DO NOT EDIT. Changes will be overwritten on next publish. -->
# claude-code-plugins

A collection of 28 Claude Code plugins organized as a marketplace catalog.

![Plugins](https://img.shields.io/badge/plugins-28-blue) ![License: MIT](https://img.shields.io/badge/License-MIT-green)

## Overview

Claude Code plugins extend the Claude Code CLI with specialized tools — each plugin provides domain-specific commands that agents can use autonomously. This repository serves as the marketplace catalog registry, listing all available plugins with their metadata and versions.

Each plugin lives in its own repository with full documentation, setup instructions, and configuration templates. The `.claude-plugin/marketplace.json` file in this repo is the canonical index.

## Quick Start

To install any plugin from the catalog:

```bash
# 1. Clone the plugin repository
git clone https://github.com/bigl34/<plugin-repo-name>.git

# 2. Configure credentials
cp config.template.json config.json  # fill in your API credentials

# 3. Install dependencies
cd scripts && npm install
```

See each plugin's README for detailed setup instructions and available commands.

## Available Plugins

### Productivity & Business Tools (21 plugins)

| Plugin                                                                                    | Version | Description                                                                                                                |
| ----------------------------------------------------------------------------------------- | ------- | -------------------------------------------------------------------------------------------------------------------------- |
| [airtable-manager](https://github.com/bigl34/claude-code-plugin-airtable)                 | 1.1.9   | Airtable database operations with isolated MCP access                                                                      |
| [betting-markets-manager](https://github.com/bigl34/claude-code-plugin-betting-markets)   | 1.3.0   | Search and aggregate prediction markets (Polymarket, Kalshi, Betfair) with unified odds and volume                         |
| [clarity-fm-manager](https://github.com/bigl34/claude-code-plugin-clarity-fm)             | 1.2.3   | Find and book expert calls on Clarity.fm via CLI-based browser automation (zero context overhead)                          |
| [clickup-task-manager](https://github.com/bigl34/claude-code-plugin-clickup)              | 1.1.9   | ClickUp task management and sprint tracking                                                                                |
| [freightos-shipment-manager](https://github.com/bigl34/claude-code-plugin-freightos)      | 1.0.11  | Freightos freight quotes (API) and booking/tracking (browser)                                                              |
| [google-workspace-manager](https://github.com/bigl34/claude-code-plugin-google-workspace) | 1.7.1   | Business Google Workspace (Gmail, Calendar, Drive, Docs, Sheets, Rich Text, Comments, Suggestions)                         |
| [gorgias-support-manager](https://github.com/bigl34/claude-code-plugin-gorgias)           | 1.1.11  | Gorgias helpdesk operations (tickets, customers, messages)                                                                 |
| [inflow-inventory-manager](https://github.com/bigl34/claude-code-plugin-inflow)           | 1.7.2   | inFlow Inventory stock management and operations                                                                           |
| [italki-manager](https://github.com/bigl34/claude-code-plugin-italki)                     | 1.2.3   | italki Mandarin Chinese teacher search, indexing, and lesson booking via hybrid HTTP API + browser automation              |
| [judgeme-review-manager](https://github.com/bigl34/claude-code-plugin-judgeme)            | 1.1.10  | Judge.me product reviews and ratings management                                                                            |
| [klaviyo-marketing-manager](https://github.com/bigl34/claude-code-plugin-klaviyo)         | 1.2.9   | Klaviyo email marketing (campaigns, flows, segments, profiles)                                                             |
| [make-scenario-manager](https://github.com/bigl34/claude-code-plugin-make)                | 1.0.9   | Trigger Make.com On-Demand scenarios (only On-Demand scheduled scenarios are exposed)                                      |
| [notion-workspace-manager](https://github.com/bigl34/claude-code-plugin-notion)           | 1.1.10  | Notion workspace documentation and SOPs                                                                                    |
| [outlook-email-manager](https://github.com/bigl34/claude-code-plugin-outlook)             | 1.2.7   | Personal Outlook/MS365 email and calendar operations                                                                       |
| [retently-feedback-manager](https://github.com/bigl34/claude-code-plugin-retently)        | 1.0.6   | Retently NPS/CSAT feedback operations (customers, responses, scores, campaigns)                                            |
| [shopify-order-manager](https://github.com/bigl34/claude-code-plugin-shopify)             | 1.1.12  | Shopify e-commerce operations (orders, customers, products)                                                                |
| [slack-manager](https://github.com/bigl34/claude-code-plugin-slack)                       | 1.1.12  | Slack workspace operations (channels, messages, users)                                                                     |
| uk-transport-manager                                                                      | 1.2.0   | UK train departures, timetables, journey planning with connections, and booking links via TransportAPI + Google Routes API |
| [web-search-manager](https://github.com/bigl34/claude-code-plugin-web-search)             | 1.1.4   | Web search and page fetching via Brave Search API and Jina Reader                                                          |
| [xero-accounting-manager](https://github.com/bigl34/claude-code-plugin-xero)              | 2.2.0   | Xero accounting operations via direct API (invoices, contacts, payments, reports, quotes, and more)                        |
| [zapier-automation-manager](https://github.com/bigl34/claude-code-plugin-zapier)          | 1.1.6   | Zapier actions + Zap management via browser automation                                                                     |

### Logistics & Shipping (5 plugins)

| Plugin                                                                               | Version | Description                                                                                                 |
| ------------------------------------------------------------------------------------ | ------- | ----------------------------------------------------------------------------------------------------------- |
| [aftership-tracking-manager](https://github.com/bigl34/claude-code-plugin-aftership) | 1.1.6   | AfterShip shipment tracking (query, monitor, retrack)                                                       |
| [easypost-shipping-manager](https://github.com/bigl34/claude-code-plugin-easypost)   | 1.0.6   | Create UPS shipping labels via EasyPost API with Shopify integration                                        |
| [royalmail-label-manager](https://github.com/bigl34/claude-code-plugin-royalmail)    | 1.0.4   | Royal Mail Click & Drop shipping labels via browser automation                                              |
| [shipsgo-container-tracker](https://github.com/bigl34/claude-code-plugin-shipsgo)    | 1.0.8   | ShipsGo ocean container tracking (API v2) - BL/container/booking tracking, ETA monitoring, vessel positions |
| [ups-collection-manager](https://github.com/bigl34/claude-code-plugin-ups)           | 2.1.6   | UPS collection booking via CLI-based browser automation (zero context overhead)                             |

### Analytics & Reporting (1 plugin)

| Plugin                                                                                    | Version | Description                                                       |
| ----------------------------------------------------------------------------------------- | ------- | ----------------------------------------------------------------- |
| [google-analytics-manager](https://github.com/bigl34/claude-code-plugin-google-analytics) | 1.3.7   | Google Analytics 4, Search Console, and Merchant Center analytics |

### Development Tools (1 plugin)

| Plugin                                                                | Version | Description                                            |
| --------------------------------------------------------------------- | ------- | ------------------------------------------------------ |
| [github-manager](https://github.com/bigl34/claude-code-plugin-github) | 1.1.6   | GitHub repository, issue, and PR management via gh CLI |

## Architecture

Each plugin follows a consistent structure:

```
plugin-name/
  .claude-plugin/
    plugin.json          # Plugin metadata and version
  agents/
    plugin-name.md       # Agent instructions and command reference
  scripts/
    cli.ts               # CLI entry point
    client.ts            # API client implementation
    package.json         # Dependencies
    config.template.json # Credential template
```

Plugins use one of two architectures:
- **MCP Wrapper** — wraps an MCP (Model Context Protocol) server binary, translating CLI commands into MCP tool calls
- **Direct API** — connects directly to the service's HTTP API, handling authentication, pagination, and error handling

## Shared Dependencies

Plugins share common utilities via these library packages:

| Library                                                                 | Purpose                                                     |
| ----------------------------------------------------------------------- | ----------------------------------------------------------- |
| [shared/cache](https://github.com/bigl34/claude-code-plugin-cache)      | Response caching with TTL and key-based invalidation        |
| [shared/cli-utils](https://github.com/bigl34/claude-code-plugin-shared) | CLI argument parsing, Zod validation, and output formatting |

## Contributing

Issues and pull requests are welcome.

## License

MIT
