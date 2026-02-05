# claude-code-plugins

A centralized marketplace and registry for Claude Code plugins, enabling extended capabilities through isolated MCP access and third-party integrations.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

## What is this?

This repository serves as the official registry for **Claude Code** plugins. It provides a structured collection of tools that extend the functionality of the Claude Code CLI agent. Each plugin is designed to handle specific tasks--from database management and shipping logistics to email automation and analytics--allowing users to customize their AI assistant's capabilities.

## Available Plugins

| Name | Description | Category |
|------|-------------|----------|
| **airtable-manager** | Airtable database operations with isolated MCP access | productivity |
| **outlook-email-manager** | Personal Outlook/MS365 email and calendar operations | productivity |
| **inflow-inventory-manager** | inFlow Inventory stock management and operations | productivity |
| **clickup-task-manager** | ClickUp task management and sprint tracking | productivity |
| **github-manager** | GitHub repository, issue, and PR management via gh CLI | development |
| **google-workspace-manager** | Business Google Workspace (Gmail, Calendar, Drive, Docs, Sheets) | productivity |
| **google-analytics-manager** | Google Analytics 4, Search Console, and Merchant Center analytics | analytics |
| **notion-workspace-manager** | Notion workspace documentation and SOPs | productivity |
| **shopify-order-manager** | Shopify e-commerce operations (orders, customers, products) | productivity |
| **web-search-manager** | Web search via Brave Search API | productivity |
| **slack-manager** | Slack workspace operations (channels, messages, users) | productivity |
| **make-scenario-manager** | Trigger Make.com On-Demand scenarios | productivity |
| **klaviyo-marketing-manager** | Klaviyo email marketing (campaigns, flows, segments, profiles) | productivity |
| **zapier-automation-manager** | Zapier actions + Zap management via browser automation | productivity |
| **gorgias-support-manager** | Gorgias helpdesk operations (tickets, customers, messages) | productivity |
| **judgeme-review-manager** | Judge.me product reviews and ratings management | productivity |
| **xero-accounting-manager** | Xero accounting operations via direct API | productivity |
| **freightos-shipment-manager** | Freightos freight quotes and booking/tracking | productivity |
| **ups-collection-manager** | UPS collection booking via CLI-based browser automation | logistics |
| **royalmail-label-manager** | Royal Mail Click & Drop shipping labels via browser automation | logistics |
| **easypost-shipping-manager** | Create UPS shipping labels via EasyPost API | logistics |
| **aftership-tracking-manager** | AfterShip shipment tracking (query, monitor, retrack) | logistics |
| **shipsgo-container-tracker** | ShipsGo ocean container tracking - BL/container/booking tracking, ETA monitoring | logistics |
| **retently-feedback-manager** | Retently NPS/CSAT feedback operations | productivity |
| **betting-markets-manager** | Search and aggregate prediction markets (Polymarket, Kalshi, Betfair) | productivity |
| **clarity-fm-manager** | Find and book expert calls on Clarity.fm via browser automation | productivity |
| **italki-manager** | italki language teacher search, indexing, and lesson booking | productivity |

## Getting Started

To use these plugins, you need to have the Claude Code CLI environment set up.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-org/claude-code-plugins.git
    cd claude-code-plugins
    ```

2.  **Browse Plugins:**
    Check `marketplace.json` for the most up-to-date list of registered plugins and their versions.

3.  **Install a Plugin:**
    Register a plugin by referencing its directory or adding it to your local configuration.

## Plugin Structure

A standard plugin in this marketplace follows this directory layout:

```text
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # Plugin manifest (name, version, description)
├── agents/
│   └── plugin-name.md   # Agent definition (commands, workflows, examples)
├── scripts/
│   ├── src/             # TypeScript source
│   ├── dist/            # Compiled JavaScript
│   ├── package.json     # Dependencies
│   └── tsconfig.json    # TypeScript config
├── config.template.json # Credential template
└── README.md            # Plugin documentation
```

## Adding Your Own Plugin

1.  **Create your plugin directory** following the structure above.
2.  **Define `plugin.json`** in `.claude-plugin/` with name, version, and description.
3.  **Write the agent doc** in `agents/` describing available commands and workflows.
4.  **Implement your CLI** in `scripts/` using TypeScript.
5.  **Update `marketplace.json`**: Add your plugin entry to the `plugins` array.
6.  **Submit a Pull Request** with your new plugin folder and the updated manifest.

## Plugin Categories

Plugins are organized into specific categories to help users find tools relevant to their workflow:

*   **Productivity:** Tools for general business operations, email, task management, and documentation (e.g., Slack, Notion, Airtable).
*   **Logistics:** Specialized tools for shipping, freight tracking, and label generation (e.g., UPS, EasyPost).
*   **Development:** Tools for software engineering tasks, version control, and code management (e.g., GitHub).
*   **Analytics:** Tools for data analysis, reporting, and web traffic monitoring (e.g., Google Analytics).

## Contributing

Issues and pull requests are welcome.

## License

MIT
