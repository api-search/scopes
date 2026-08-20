---
authorization_urls: []
description: ''
docs: https://www.raindrop.ai/docs/mcp/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Raindrop Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by Raindrop's PropelAuth-backed authorization server (used for MCP OAuth 2.1 and dashboard sign-in). The ingest and query REST APIs use bearer API keys rather than OAuth scopes.
overview: 'Raindrop uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Raindrop
provider_slug: raindrop
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: raindrop-scopes
source_filename: raindrop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.raindrop.ai/.well-known/openid-configuration\nflow: authorization_code\nissuer: https://auth.raindrop.ai\ndocs: https://www.raindrop.ai/docs/mcp/overview\nnote: >-\n  OAuth/OIDC scopes advertised by Raindrop's PropelAuth-backed authorization\n  server (used for MCP OAuth 2.1 and dashboard sign-in). The ingest and query\n  REST APIs use bearer API keys rather than OAuth scopes.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; returns an ID token.\n- name: email\n  description: Access to the user's email address and verification status.\n- name: profile\n  description: Access to basic profile claims (first_name, last_name, picture_url).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raindrop/refs/heads/main/scopes/raindrop-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Agents
- Observability
- Monitoring
- LLMOps
- Developer Tools
- Tracing
token_urls: []
---
