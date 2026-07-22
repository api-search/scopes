---
authorization_urls: []
description: OAuth 2.0 scopes advertised by Zatanna's authorization server (RFC 8414 metadata) and echoed by the MCP protected-resource metadata (RFC 9728). These are OpenID Connect standard scopes plus offline_access for refresh tokens; no Zatanna-specific resource scopes are published anonymously. No OpenAPI is available, so scopes are taken verbatim from the discovery documents.
docs: https://api.zatanna.ai/.well-known/oauth-protected-resource
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Zatanna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zatanna publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zatanna API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zatanna
provider_slug: zatanna
schemes:
- authorizationUrl: https://api.zatanna.ai/api/auth/mcp/authorize
  authorization_server: https://api.zatanna.ai
  grant_types:
  - authorization_code
  - refresh_token
  name: Zatanna MCP OAuth
  protected_resource: well-known/zatanna-mcp-oauth-protected-resource.json
  tokenUrl: https://api.zatanna.ai/api/auth/mcp/token
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issues an RS256-signed ID token identifying the subject.
  flows: []
  scope: openid
- description: Access to the end user's basic profile claims (e.g. name).
  flows: []
  scope: profile
- description: Access to the end user's email and email_verified claims.
  flows: []
  scope: email
- description: Grants a refresh token so the client can obtain new access tokens without user interaction.
  flows: []
  scope: offline_access
slug: zatanna-scopes
source_filename: zatanna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.zatanna.ai/.well-known/oauth-authorization-server\ndocs: https://api.zatanna.ai/.well-known/oauth-protected-resource\ndescription: >-\n  OAuth 2.0 scopes advertised by Zatanna's authorization server (RFC 8414\n  metadata) and echoed by the MCP protected-resource metadata (RFC 9728). These\n  are OpenID Connect standard scopes plus offline_access for refresh tokens; no\n  Zatanna-specific resource scopes are published anonymously. No OpenAPI is\n  available, so scopes are taken verbatim from the discovery documents.\nschemes:\n  - name: Zatanna MCP OAuth\n    type: oauth2\n    grant_types: [authorization_code, refresh_token]\n    authorizationUrl: https://api.zatanna.ai/api/auth/mcp/authorize\n    tokenUrl: https://api.zatanna.ai/api/auth/mcp/token\n    protected_resource: well-known/zatanna-mcp-oauth-protected-resource.json\n    authorization_server: https://api.zatanna.ai\nscopes:\n  - scope: openid\n    description:\
  \ OpenID Connect authentication; issues an RS256-signed ID token identifying the subject.\n    schemes: [Zatanna MCP OAuth]\n  - scope: profile\n    description: Access to the end user's basic profile claims (e.g. name).\n    schemes: [Zatanna MCP OAuth]\n  - scope: email\n    description: Access to the end user's email and email_verified claims.\n    schemes: [Zatanna MCP OAuth]\n  - scope: offline_access\n    description: Grants a refresh token so the client can obtain new access tokens without user interaction.\n    schemes: [Zatanna MCP OAuth]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zatanna/refs/heads/main/scopes/zatanna-scopes.yml
summary_line: 4 scopes
tags:
- Company
- API
- MCP
- AI Agents
- Integration
- Reverse Engineering
- Automation
- OAuth
- Y Combinator
token_urls: []
---
