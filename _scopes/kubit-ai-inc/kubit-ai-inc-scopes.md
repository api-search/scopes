---
authorization_urls: []
description: ''
docs: https://docs.kubit.ai/docs/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Kubit Ai Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kubit AI, Inc. uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kubit AI, Inc.
provider_slug: kubit-ai-inc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kubit-ai-inc-scopes
source_filename: kubit-ai-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.kubit.ai/.well-known/oauth-authorization-server\ndocs: https://docs.kubit.ai/docs/mcp-server\nauthorization_server: https://mcp.kubit.ai\nprotected_resource: https://mcp.kubit.ai/mcp\nnotes: >-\n  Kubit's only documented OAuth surface is the hosted MCP server. The scopes below are\n  taken verbatim from the published RFC 8414 authorization-server metadata and the\n  RFC 9728 protected-resource metadata. Kubit's web platform authenticates with SSO\n  (SAML/OIDC via Google Workspace, Okta, Microsoft Entra ID, AWS IAM Identity Center)\n  and exposes no separate public scope registry.\nscopes:\n  - name: mcp:read\n    description: >-\n      Read access to Kubit analytics through the MCP server — user context, schema\n      metadata, existing report results and raw data exports, and search.\n  - name: mcp:write\n    description: >-\n      Write access through the MCP server — creating and executing new reports against\n\
  \      the connected warehouse.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubit-ai-inc/refs/heads/main/scopes/kubit-ai-inc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Analytics
- Product Analytics
- Data Warehouse
- LLM Observability
- MCP
- Agent Analytics
- OpenTelemetry
- DevOps
token_urls: []
---
