---
authorization_urls: []
description: ''
docs: https://www.raindrop.ai/docs/mcp/overview
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: searched
name: Raindrop Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by Raindrop's PropelAuth-backed authorization server (used for MCP OAuth 2.1 and dashboard sign-in). The ingest and query REST APIs use bearer API keys rather than OAuth scopes.
overview: 'Raindrop publishes 3 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Raindrop API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Raindrop
provider_slug: raindrop
schemes: []
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: Standard OpenID Connect scope; returns an ID token.
  flows: []
  scope: openid
- description: Access to the user's email address and verification status.
  flows: []
  scope: email
- description: Access to basic profile claims (first_name, last_name, picture_url).
  flows: []
  scope: profile
slug: raindrop-scopes
source_filename: raindrop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.raindrop.ai/.well-known/openid-configuration\nflow: authorization_code\nissuer: https://auth.raindrop.ai\ndocs: https://www.raindrop.ai/docs/mcp/overview\nnote: >-\n  OAuth/OIDC scopes advertised by Raindrop's PropelAuth-backed authorization\n  server (used for MCP OAuth 2.1 and dashboard sign-in). The ingest and query\n  REST APIs use bearer API keys rather than OAuth scopes.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; returns an ID token.\n- name: email\n  description: Access to the user's email address and verification status.\n- name: profile\n  description: Access to basic profile claims (first_name, last_name, picture_url).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raindrop/refs/heads/main/scopes/raindrop-scopes.yml
summary_line: 3 scopes · authorization_code
tags:
- Company
- Artificial Intelligence
- Agents
- Observability
- Monitoring
- LLMOps
- Developer Tools
- Tracing
token_bound: false
token_urls: []
---
