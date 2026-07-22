---
authorization_urls:
- https://discovery.matchory.com/auth/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Matchory Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Matchory publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Matchory API on a user''s behalf.


  Tokens are issued from https://discovery.matchory.com/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Matchory
provider_slug: matchory
schemes:
- flows:
  - authorizationUrl: https://discovery.matchory.com/auth/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://discovery.matchory.com/auth/oauth/token
  - flow: clientCredentials
    tokenUrl: https://discovery.matchory.com/auth/oauth/token
  name: OAuth2
  source: well-known/matchory-openid-configuration.json
scope_count: 4
scope_names:
- openid
- profile
- email
- mcp:use
scopes:
- description: OpenID Connect authentication; issue an ID token for the subject.
  flows:
  - authorizationCode
  scope: openid
- description: Access the end-user's basic profile claims (name, given_name, family_name, picture, locale).
  flows:
  - authorizationCode
  scope: profile
- description: Access the end-user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Authorize a client to call Matchory's OAuth-protected MCP server at https://discovery.matchory.com/mcp (advertised as the required scope in the RFC 9728 protected-resource metadata).
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:use
slug: matchory-scopes
source_filename: matchory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://discovery.matchory.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: well-known/matchory-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discovery.matchory.com/auth/oauth/authorize\n    tokenUrl: https://discovery.matchory.com/auth/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://discovery.matchory.com/auth/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the subject.\n  flows: [authorizationCode]\n  sources: [well-known/matchory-openid-configuration.json]\n- scope: profile\n  description: Access the end-user's basic profile claims (name, given_name, family_name, picture, locale).\n  flows: [authorizationCode]\n  sources: [well-known/matchory-openid-configuration.json]\n- scope: email\n  description: Access the end-user's email and email_verified claims.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/matchory-openid-configuration.json]\n- scope: mcp:use\n  description: >-\n    Authorize a client to call Matchory's OAuth-protected MCP server at\n    https://discovery.matchory.com/mcp (advertised as the required scope in the\n    RFC 9728 protected-resource metadata).\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/matchory-oauth-protected-resource.json, well-known/matchory-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matchory/refs/heads/main/scopes/matchory-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Procurement
- Supplier Discovery
- Sourcing
- Supply Chain
- Data Enrichment
- Entity Resolution
- Market Intelligence
- Risk Management
- MCP
token_urls:
- https://discovery.matchory.com/auth/oauth/token
---
