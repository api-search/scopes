---
authorization_urls:
- https://mcp.conviva.com/oauth/authorize
- https://dpi-mcp.conviva.com/oauth/authorize
description: Conviva's only OAuth surface is its two hosted MCP servers. The REST surface at api.conviva.com is HTTP Basic with an API key pair and has NO scope model at all — REST authorization is by c3 account plus product entitlement (e.g. Precision Admin), not by scope. The scopes below are taken verbatim from the live RFC 8414 / RFC 9728 discovery documents; Conviva publishes no human-readable scope reference page, so the descriptions are the standard OIDC meanings and the Conviva-specific `conviva` scope is recorded without an official description rather than guessed.
docs: https://docs.conviva.ai/connect-data/mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Conviva Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Conviva publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conviva API on a user''s behalf.


  Tokens are issued from https://mcp.conviva.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conviva
provider_slug: conviva
schemes:
- flows:
  - authorizationUrl: https://mcp.conviva.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://mcp.conviva.com/oauth/register
    tokenUrl: https://mcp.conviva.com/oauth/token
  name: convivaMcpOAuth
  server: https://mcp.conviva.com
  source: https://mcp.conviva.com/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://dpi-mcp.conviva.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://dpi-mcp.conviva.com/oauth/register
    tokenUrl: https://dpi-mcp.conviva.com/oauth/token
  identity_provider: Okta
  name: convivaDpiMcpOAuth
  server: https://dpi-mcp.conviva.com
  source: https://dpi-mcp.conviva.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- conviva
scopes:
- description: OpenID Connect — request an ID token identifying the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: conviva
slug: conviva-scopes
source_filename: conviva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://mcp.conviva.com/.well-known/oauth-authorization-server\ndocs: https://docs.conviva.ai/connect-data/mcp/\ndescription: >-\n  Conviva's only OAuth surface is its two hosted MCP servers. The REST surface at api.conviva.com\n  is HTTP Basic with an API key pair and has NO scope model at all — REST authorization is by c3\n  account plus product entitlement (e.g. Precision Admin), not by scope. The scopes below are\n  taken verbatim from the live RFC 8414 / RFC 9728 discovery documents; Conviva publishes no\n  human-readable scope reference page, so the descriptions are the standard OIDC meanings and the\n  Conviva-specific `conviva` scope is recorded without an official description rather than guessed.\n\nschemes:\n- name: convivaMcpOAuth\n  server: https://mcp.conviva.com\n  source: https://mcp.conviva.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.conviva.com/oauth/authorize\n\
  \    tokenUrl: https://mcp.conviva.com/oauth/token\n    registrationUrl: https://mcp.conviva.com/oauth/register\n    code_challenge_methods: [S256]\n- name: convivaDpiMcpOAuth\n  server: https://dpi-mcp.conviva.com\n  source: https://dpi-mcp.conviva.com/.well-known/oauth-authorization-server\n  identity_provider: Okta\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dpi-mcp.conviva.com/oauth/authorize\n    tokenUrl: https://dpi-mcp.conviva.com/oauth/token\n    registrationUrl: https://dpi-mcp.conviva.com/oauth/register\n    code_challenge_methods: [S256]\n\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token identifying the authenticated user.\n  flows: [authorizationCode]\n  advertised_in: [oauth-authorization-server, oauth-protected-resource]\n  sources: [https://mcp.conviva.com, https://dpi-mcp.conviva.com]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n  advertised_in: [oauth-authorization-server,\
  \ oauth-protected-resource]\n  sources: [https://mcp.conviva.com, https://dpi-mcp.conviva.com]\n- scope: email\n  description: Access to the user's email claim.\n  flows: [authorizationCode]\n  advertised_in: [oauth-authorization-server, oauth-protected-resource]\n  sources: [https://mcp.conviva.com, https://dpi-mcp.conviva.com]\n- scope: conviva\n  description: null\n  description_note: >-\n    Conviva-specific resource scope. Advertised in the protected-resource metadata\n    (scopes_supported) and in the /mcp service descriptor's oauth.scopes, but NOT in the\n    authorization-server metadata's scopes_supported, and Conviva publishes no scope reference\n    page. Its exact grant semantics are undocumented — recorded, not guessed.\n  flows: [authorizationCode]\n  advertised_in: [oauth-protected-resource, service-descriptor]\n  sources: [https://mcp.conviva.com, https://dpi-mcp.conviva.com]\n\ndiscovery_discrepancy: >-\n  /.well-known/oauth-authorization-server lists scopes_supported\
  \ [openid, profile, email] while\n  /.well-known/oauth-protected-resource lists [openid, profile, email, conviva] and the GET /mcp\n  service descriptor lists [openid, profile, conviva]. The three published lists disagree; the\n  union is recorded above with per-scope provenance.\n\nprotected_resources:\n- resource: https://mcp.conviva.com\n  resource_name: mcp-server-conviva\n  authorization_servers: [https://mcp.conviva.com]\n  resource_documentation: https://mcp.conviva.com/health\n- resource: https://dpi-mcp.conviva.com\n  resource_name: mcp-server-conviva\n  authorization_servers: [https://dpi-mcp.conviva.com]\n  resource_documentation: https://dpi-mcp.conviva.com/health\n\nrest_authorization_model:\n  scheme: 'HTTP Basic (client-id : client-secret)'\n  scopes: none\n  unit_of_authorization: c3 account\n  entitlements:\n  - name: Precision Admin\n    effect: Required to create the credentials used for Precision Policy POST operations; without it\n      the API returns 403 Forbidden.\n\
  \  - name: Precision API activation\n    effect: Precision APIs must be activated for the c3 account, with edit permissions.\n\nx-evidence:\n  fetched: '2026-08-01'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conviva/refs/heads/main/scopes/conviva-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Analytics
- Streaming
- Video
- Observability
- Monitoring
- Media
- Quality of Experience
- Real Time
- Telemetry
- Agents
- MCP
- Company
token_urls:
- https://mcp.conviva.com/oauth/token
- https://dpi-mcp.conviva.com/oauth/token
---
