---
authorization_urls: []
description: ''
docs: https://docs.marcopolo.dev/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Marco Polo Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the MarcoPolo authorization server (WorkOS AuthKit) via RFC 8414 metadata. These are the standard OIDC/OAuth scopes; MarcoPolo does not publish application-specific resource scopes.
overview: 'Marco Polo publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Marco Polo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Marco Polo
provider_slug: marco-polo
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in; issue an ID token.
  flows: []
  scope: openid
- description: Access the user's basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: marco-polo-scopes
source_filename: marco-polo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.marcopolo.dev/.well-known/oauth-authorization-server\nprovider: marco-polo\ndocs: https://docs.marcopolo.dev/getting-started\nnote: >-\n  Scopes advertised by the MarcoPolo authorization server (WorkOS AuthKit) via\n  RFC 8414 metadata. These are the standard OIDC/OAuth scopes; MarcoPolo does not\n  publish application-specific resource scopes.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; issue an ID token.\n- name: profile\n  description: Access the user's basic profile claims.\n- name: email\n  description: Access the user's email address.\n- name: offline_access\n  description: Issue a refresh token for long-lived access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marco-polo/refs/heads/main/scopes/marco-polo-scopes.yml
summary_line: 4 scopes
tags:
- Company
- MCP
- Enterprise AI
- Data Governance
- AI Agents
- Data Integration
- Security
- Authentication
token_bound: false
token_urls: []
---
