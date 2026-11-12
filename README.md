# Armiqo Brain

**Free B2B account management playbook for AI assistants.**

Connect Armiqo Brain to an MCP-compatible AI assistant to get practical guidance on retaining clients, preparing account reviews, planning renewals, identifying churn signals and growing existing relationships.

**[Connect Armiqo Brain](https://armiqo.com/brain/)** · **[MCP endpoint](https://armiqo.com/mcp/)**

## What you get

- Account plans built around customer goals
- Early-warning prompts for retention and churn risk
- Renewal and expansion conversation frameworks
- Meeting and QBR preparation
- Stakeholder mapping and difficult-client scenarios

The Brain is an **on-demand, read-only knowledge resource**. It cannot access your CRM, monitor accounts, send emails, schedule reminders, or take actions without additional integrations.

## Connect

Remote MCP URL:

```text
https://armiqo.com/mcp/
```

Use your assistant's **Add MCP server / Connectors** interface and select a remote HTTP MCP server. Availability and exact steps depend on your app and subscription. For Claude Desktop, ChatGPT and other clients, follow that client's current remote-MCP setup flow.

No Armiqo login is currently required.

### Try these questions

- "A client stopped responding 90 days before renewal. What should I check first?"
- "Help me prepare a quarterly business review for an agency client."
- "How do I raise rates without damaging a long-term client relationship?"
- "Create a 90-day account plan based on my client's goals."

Do not include customer secrets or personal data in questions. Your AI client chooses what arguments it sends to the MCP server.

## MCP tools

| Tool | Purpose |
| --- | --- |
| `consult_brain` | Route a question to relevant playbook modules |
| `list_modules` | Show available modules |
| `get_module` | Retrieve a module |

## Source and licensing

**This repository is the public integration, metadata and documentation package, not the source of the hosted MCP implementation.** The hosted server, analytics integration and full playbook content remain private for now. The MIT license in this repository applies to the files actually published here. It does not cover the private hosted implementation or its proprietary playbook content.

If we later release a sanitized self-hostable edition, it will have its own clear license and compatibility notes. Do not copy the private monorepo, internal research, customer materials or build-time-generated playbook text into this repo.

## Privacy

The server can receive the questions an AI client forwards to the `consult_brain` tool. Usage analytics may record the tool name, inferred topic, anonymous usage identifiers, errors and response time. The server's telemetry implementation is designed not to send raw questions or response bodies to PostHog.

Read the [Armiqo website](https://armiqo.com/brain/) for the current product description.

## Report a problem

Open a GitHub issue with steps to reproduce, your MCP client name/version, and a sanitized error message. Never paste access tokens, customer names, confidential client details or private chats.

## About Armiqo

Armiqo Brain is a free educational entry point to [Armiqo](https://armiqo.com/), a system for running proactive post-sale account management.
