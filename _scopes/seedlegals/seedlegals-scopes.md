---
authorization_urls:
- https://api.seedlegals.com/mcp/oauth2/authorize
- https://auth.seedlegals.com/oauth2/authorize
description: ''
docs: https://api.seedlegals.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Seedlegals Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SeedLegals publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SeedLegals API on a user''s behalf.


  Tokens are issued from https://api.seedlegals.com/mcp/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SeedLegals
provider_slug: seedlegals
schemes:
- flows:
  - authorizationUrl: https://api.seedlegals.com/mcp/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.seedlegals.com/mcp/oauth2/token
  name: SeedLegals MCP OAuth2
  source: https://api.seedlegals.com/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://auth.seedlegals.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.seedlegals.com/oauth2/token
  name: SeedLegals Identity (FusionAuth OIDC)
  source: https://auth.seedlegals.com/.well-known/openid-configuration
scope_count: 7
scope_names:
- openid
- email
- read
- write
- offline_access
- phone
- profile
scopes:
- description: OpenID Connect authentication; issue an ID token for the SeedLegals user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Read access to SeedLegals resources exposed through the MCP server.
  flows:
  - authorizationCode
  scope: read
- description: Write access to SeedLegals resources exposed through the MCP server.
  flows:
  - authorizationCode
  scope: write
- description: Issue a refresh token for long-lived access (FusionAuth identity provider).
  flows:
  - authorizationCode
  scope: offline_access
- description: Access the authenticated user's phone number (FusionAuth identity provider).
  flows:
  - authorizationCode
  scope: phone
- description: Access the authenticated user's profile claims (FusionAuth identity provider).
  flows:
  - authorizationCode
  scope: profile
slug: seedlegals-scopes
source_filename: seedlegals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.seedlegals.com/.well-known/oauth-authorization-server\ndocs: https://api.seedlegals.com/.well-known/oauth-protected-resource\nschemes:\n- name: SeedLegals MCP OAuth2\n  source: https://api.seedlegals.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.seedlegals.com/mcp/oauth2/authorize\n    tokenUrl: https://api.seedlegals.com/mcp/oauth2/token\n- name: SeedLegals Identity (FusionAuth OIDC)\n  source: https://auth.seedlegals.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.seedlegals.com/oauth2/authorize\n    tokenUrl: https://auth.seedlegals.com/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the SeedLegals user.\n  flows: [authorizationCode]\n  sources: [MCP OAuth2, FusionAuth OIDC]\n- scope: email\n  description: Access the\
  \ authenticated user's email address.\n  flows: [authorizationCode]\n  sources: [MCP OAuth2, FusionAuth OIDC]\n- scope: read\n  description: Read access to SeedLegals resources exposed through the MCP server.\n  flows: [authorizationCode]\n  sources: [MCP OAuth2]\n- scope: write\n  description: Write access to SeedLegals resources exposed through the MCP server.\n  flows: [authorizationCode]\n  sources: [MCP OAuth2]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access (FusionAuth identity provider).\n  flows: [authorizationCode]\n  sources: [FusionAuth OIDC]\n- scope: phone\n  description: Access the authenticated user's phone number (FusionAuth identity provider).\n  flows: [authorizationCode]\n  sources: [FusionAuth OIDC]\n- scope: profile\n  description: Access the authenticated user's profile claims (FusionAuth identity provider).\n  flows: [authorizationCode]\n  sources: [FusionAuth OIDC]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seedlegals/refs/heads/main/scopes/seedlegals-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Business Applications
- Legal Tech
- Startups
- Fundraising
- Cap Table
- Equity
- Compliance
- MCP
- OpenID Connect
token_urls:
- https://api.seedlegals.com/mcp/oauth2/token
- https://auth.seedlegals.com/oauth2/token
---
