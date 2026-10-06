# OpenPost agent plugin

Prepare and review social posts through OpenPost's authenticated MCP server. This package contains client configuration and one operating skill. The server and product source live in [getopenpost/openpost](https://github.com/getopenpost/openpost).

## Connect

Install this repository as a plugin in a compatible client. Cursor reads `.cursor-plugin/plugin.json`; Claude-compatible clients and Grok Build read `.claude-plugin/plugin.json`. Both use the root `.mcp.json`.

Sign in to OpenPost when the client starts OAuth. Choose read-only access for schedule, account, and delivery inspection. Grant change access only when you want the agent to prepare or modify content. The plugin contains no token, saved session, or account data.

Hosted registration currently uses a waitlist. Existing Hosted users can sign in. Self-hosted users can change the MCP URL to their own public HTTPS endpoint. See [MCP setup](https://openpo.st/docs/mcp).

## Use

Ask the agent to list your workspaces, name one, and review its schedule without changes. For a draft, specify the source idea and destinations. Review the saved variants before approving a schedule or publication.

The operating skill preserves provider readiness and actual delivery states. It does not claim that every integration supports every format, inbox operation, or metric. Connected browser editors have their own requirements and are not advertised by this plugin.

## Scope

This repository packages the maintained OpenPost service for agent marketplaces. It is not a standalone MCP server, a server deployment, or a Grok Bot template. [OpenPost](https://openpo.st) owns the product, service, and API contracts.

License: AGPL-3.0-only. The OpenPost Converge mark remains the product's brand.
