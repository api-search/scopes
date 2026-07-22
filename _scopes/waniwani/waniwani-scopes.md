---
authorization_urls: []
description: ''
docs: https://docs.waniwani.ai/mcp-server/how-it-works
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Waniwani Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Waniwani publishes 25 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Waniwani API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Waniwani
provider_slug: waniwani
schemes:
- authorization_servers:
  - https://app.waniwani.ai
  bearer_methods:
  - header
  name: OAuth2.1
  resource: https://mcp.waniwani.ai/mcp
  source: https://mcp.waniwani.ai/.well-known/oauth-protected-resource
scope_count: 25
scope_names:
- mcp:tools
- openid
- profile
- email
- offline_access
- orgs:read
- orgs:write
- mcp:read
- mcp:write
- kb:read
- kb:write
- analytics:read
- analytics:write
- evals:read
- evals:write
- conversations:read
- conversations:write
- competition:read
- competition:write
- geo:read
- geo:write
- connectors:read
- connectors:write
- superadmin:read
- superadmin:write
scopes:
- description: Invoke the hosted MCP server's tools.
  flows: []
  scope: mcp:tools
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access basic profile information.
  flows: []
  scope: profile
- description: Access the account email address.
  flows: []
  scope: email
- description: Obtain refresh tokens for long-lived access.
  flows: []
  scope: offline_access
- description: Read organization details.
  flows: []
  scope: orgs:read
- description: Manage organizations.
  flows: []
  scope: orgs:write
- description: Read MCP server resources.
  flows: []
  scope: mcp:read
- description: Modify MCP server resources.
  flows: []
  scope: mcp:write
- description: Read knowledge base content.
  flows: []
  scope: kb:read
- description: Write knowledge base content.
  flows: []
  scope: kb:write
- description: Read funnel analytics and digests.
  flows: []
  scope: analytics:read
- description: Manage analytics configuration.
  flows: []
  scope: analytics:write
- description: Read synthetic-buyer / evaluation results.
  flows: []
  scope: evals:read
- description: Manage synthetic-buyer / evaluation runs.
  flows: []
  scope: evals:write
- description: Read conversation and session data.
  flows: []
  scope: conversations:read
- description: Manage conversation and session data.
  flows: []
  scope: conversations:write
- description: Read competitive / market-visibility data.
  flows: []
  scope: competition:read
- description: Manage competitive-monitoring configuration.
  flows: []
  scope: competition:write
- description: Read geo / jurisdiction data.
  flows: []
  scope: geo:read
- description: Manage geo / jurisdiction configuration.
  flows: []
  scope: geo:write
- description: Read connector / integration configuration.
  flows: []
  scope: connectors:read
- description: Manage connectors / integrations.
  flows: []
  scope: connectors:write
- description: Elevated read access (administrative).
  flows: []
  scope: superadmin:read
- description: Elevated write access (administrative).
  flows: []
  scope: superadmin:write
slug: waniwani-scopes
source_filename: waniwani-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.waniwani.ai/.well-known/oauth-protected-resource\ndocs: https://docs.waniwani.ai/mcp-server/how-it-works\nschemes:\n  - name: OAuth2.1\n    source: https://mcp.waniwani.ai/.well-known/oauth-protected-resource\n    authorization_servers: [https://app.waniwani.ai]\n    resource: https://mcp.waniwani.ai/mcp\n    bearer_methods: [header]\nscopes:\n  - {scope: \"mcp:tools\", description: \"Invoke the hosted MCP server's tools.\"}\n  - {scope: \"openid\", description: \"OpenID Connect authentication.\"}\n  - {scope: \"profile\", description: \"Access basic profile information.\"}\n  - {scope: \"email\", description: \"Access the account email address.\"}\n  - {scope: \"offline_access\", description: \"Obtain refresh tokens for long-lived access.\"}\n  - {scope: \"orgs:read\", description: \"Read organization details.\"}\n  - {scope: \"orgs:write\", description: \"Manage organizations.\"}\n  - {scope: \"mcp:read\", description:\
  \ \"Read MCP server resources.\"}\n  - {scope: \"mcp:write\", description: \"Modify MCP server resources.\"}\n  - {scope: \"kb:read\", description: \"Read knowledge base content.\"}\n  - {scope: \"kb:write\", description: \"Write knowledge base content.\"}\n  - {scope: \"analytics:read\", description: \"Read funnel analytics and digests.\"}\n  - {scope: \"analytics:write\", description: \"Manage analytics configuration.\"}\n  - {scope: \"evals:read\", description: \"Read synthetic-buyer / evaluation results.\"}\n  - {scope: \"evals:write\", description: \"Manage synthetic-buyer / evaluation runs.\"}\n  - {scope: \"conversations:read\", description: \"Read conversation and session data.\"}\n  - {scope: \"conversations:write\", description: \"Manage conversation and session data.\"}\n  - {scope: \"competition:read\", description: \"Read competitive / market-visibility data.\"}\n  - {scope: \"competition:write\", description: \"Manage competitive-monitoring configuration.\"}\n  - {scope:\
  \ \"geo:read\", description: \"Read geo / jurisdiction data.\"}\n  - {scope: \"geo:write\", description: \"Manage geo / jurisdiction configuration.\"}\n  - {scope: \"connectors:read\", description: \"Read connector / integration configuration.\"}\n  - {scope: \"connectors:write\", description: \"Manage connectors / integrations.\"}\n  - {scope: \"superadmin:read\", description: \"Elevated read access (administrative).\"}\n  - {scope: \"superadmin:write\", description: \"Elevated write access (administrative).\"}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waniwani/refs/heads/main/scopes/waniwani-scopes.yml
summary_line: 25 scopes
tags:
- Company
- Artificial Intelligence
- Model Context Protocol
- AI Distribution
- Conversational AI
- Lead Generation
- Insurance
- Fintech
- Agents
- SDK
token_urls: []
---
