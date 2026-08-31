---
authorization_urls: []
description: '6sense''s OAuth surface publishes exactly one scope. It governs the MCP server at https://api.6sense.com/mcp, not the REST APIs — those authenticate with an `Authorization: Token <api_token>` header and have no OAuth scopes. What the REST APIs scope instead is the API TOKEN itself: tokens are issued per API group and are limited by the credit type the customer purchased, and the Score and Segments settings on a token further restrict what detail it may return. That authorization model is not expressed as OAuth scopes anywhere 6sense publishes.'
docs: https://support.6sense.com/docs/6sense-model-context-protocol-mcp-1
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: 6Sense Insights Scopes
name_suffix: OAuth Scopes
note: ''
overview: '6Sense Insights uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 6Sense Insights
provider_slug: 6sense-insights
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: 6sense-insights-scopes
source_filename: 6sense-insights-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.6sense.com/.well-known/oauth-authorization-server and\n  https://api.6sense.com/.well-known/oauth-protected-resource/mcp (both fetched\n  live, HTTP 200).\ndescription: >-\n  6sense's OAuth surface publishes exactly one scope. It governs the MCP server\n  at https://api.6sense.com/mcp, not the REST APIs — those authenticate with an\n  `Authorization: Token <api_token>` header and have no OAuth scopes. What the\n  REST APIs scope instead is the API TOKEN itself: tokens are issued per API\n  group and are limited by the credit type the customer purchased, and the\n  Score and Segments settings on a token further restrict what detail it may\n  return. That authorization model is not expressed as OAuth scopes anywhere\n  6sense publishes.\ndocs: https://support.6sense.com/docs/6sense-model-context-protocol-mcp-1\nauthorization_server: >-\n  https://auth.6sense.com/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN\n\
  resource: https://api.6sense.com/mcp\nscopes:\n  - name: mcp:use\n    description: >-\n      Read-only access to 6sense data through the 6sense MCP server, scoped to\n      the 6sense instance and the user account used during authorization.\n    resource: https://api.6sense.com/mcp\n    grants: read\n    evidence: >-\n      scopes_supported [\"mcp:use\"] in both the RFC 8414 authorization-server\n      metadata and the RFC 9728 protected-resource metadata.\nscope_count: 1\nnotes:\n  - >-\n    Authorization is per user — every 6sense user must complete the consent flow\n    individually, and a connector is isolated to the instance authorized during\n    that flow.\n  - >-\n    The scope is coarse: there is no per-capability decomposition, so a client\n    granted mcp:use reaches every documented MCP capability the user's own\n    6sense entitlements allow. Entitlement, not scope, is the real boundary.\n  - >-\n    No token-scope / permission reference page is published for the REST API\n\
  \    tokens; the docs describe API groups and credit types in prose only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense-insights/refs/heads/main/scopes/6sense-insights-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Marketing Technology
- Artificial Intelligence
- Data Enrichment
token_urls: []
---
