---
authorization_urls:
- https://mcp.clearskies.cc/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Scratchpad Scopes
name_suffix: OAuth Scopes
note: 'Scopes are read from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata on the Clearskies MCP host; both advertise the same three. Clearskies publishes no scopes or permissions reference page, so there is nothing to enrich these with. The authorization surface is identity-only: the three OIDC scopes establish who the caller is, and the data a token can reach is then governed inside the workspace by the per-source connections and the permissions of the underlying system (Salesforce, HubSpot, Gong, Slack and the rest), not by an OAuth scope string. There is no read/write or per-object scope vocabulary to record.'
overview: 'Scratchpad publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Scratchpad API on a user''s behalf.


  Tokens are issued from https://mcp.clearskies.cc/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scratchpad
provider_slug: scratchpad
schemes:
- flows:
  - authorizationUrl: https://mcp.clearskies.cc/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.clearskies.cc/oauth/token
  name: ClearskiesMCPOAuth
  source: well-known/scratchpad-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect - issue an ID token identifying the subject.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the authenticated user; the Clearskies connect flow authenticates a team member by their email domain.
  flows:
  - authorizationCode
  scope: email
slug: scratchpad-scopes
source_filename: scratchpad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.clearskies.cc/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are read from the live RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata on the Clearskies MCP host; both advertise the same three. Clearskies\n  publishes no scopes or permissions reference page, so there is nothing to enrich these with. The\n  authorization surface is identity-only: the three OIDC scopes establish who the caller is, and the\n  data a token can reach is then governed inside the workspace by the per-source connections and the\n  permissions of the underlying system (Salesforce, HubSpot, Gong, Slack and the rest), not by an\n  OAuth scope string. There is no read/write or per-object scope vocabulary to record.\n\nschemes:\n- name: ClearskiesMCPOAuth\n  source: well-known/scratchpad-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.clearskies.cc/oauth/authorize\n\
  \    tokenUrl: https://mcp.clearskies.cc/oauth/token\n\nscopes:\n- scope: openid\n  description: OpenID Connect - issue an ID token identifying the subject.\n  flows: [authorizationCode]\n  sources: [well-known/scratchpad-oauth-authorization-server.json, well-known/scratchpad-oauth-protected-resource.json]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  flows: [authorizationCode]\n  sources: [well-known/scratchpad-oauth-authorization-server.json, well-known/scratchpad-oauth-protected-resource.json]\n- scope: email\n  description: Email address claim for the authenticated user; the Clearskies connect flow\n    authenticates a team member by their email domain.\n  flows: [authorizationCode]\n  sources: [well-known/scratchpad-oauth-authorization-server.json, well-known/scratchpad-oauth-protected-resource.json]\n\nscope_count: 3\n\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://mcp.clearskies.cc/.well-known/oauth-authorization-server\n  http_status:\
  \ 200\n- fetched: '2026-08-13'\n  url: https://mcp.clearskies.cc/.well-known/oauth-protected-resource\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpad/refs/heads/main/scopes/scratchpad-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Productivity
- Sales
- CRM
- Salesforce
- Revenue Operations
- Artificial Intelligence
- SaaS
- MCP
- Model Context Protocol
- Agents
- Sales Intelligence
token_urls:
- https://mcp.clearskies.cc/oauth/token
---
