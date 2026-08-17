---
api_specs:
- filename: clevertap-campaigns-api-openapi.yml
  format: yaml
  label: CleverTap Campaigns API
  slug: clevertap-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-campaigns-api-openapi.yml
- filename: clevertap-events-api-openapi.yml
  format: yaml
  label: CleverTap Events API
  slug: clevertap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-events-api-openapi.yml
- filename: clevertap-profiles-api-openapi.yml
  format: yaml
  label: CleverTap Profiles API
  slug: clevertap-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-profiles-api-openapi.yml
- filename: clevertap-reports-api-openapi.yml
  format: yaml
  label: CleverTap Reports API
  slug: clevertap-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-reports-api-openapi.yml
authorization_urls:
- https://mcp.clevertap.com/oauth/authorize
description: 'OAuth scopes CleverTap advertises. Scope applies to ONE surface only: the remote MCP server at mcp.clevertap.com. The CleverTap REST API has no OAuth and therefore no scopes — it authenticates with two static headers (X-CleverTap-Account-Id, X-CleverTap-Passcode) with no scoping, expiry or least-privilege model at all. The scopes below were read from the server''s own RFC 8414 and RFC 9728 metadata documents, not from documentation: CleverTap publishes no scopes or permissions reference page.'
docs: ''
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Clevertap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CleverTap publishes 4 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CleverTap API on a user''s behalf.


  Tokens are issued from https://mcp.clevertap.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CleverTap
provider_slug: clevertap
schemes:
- flows:
  - authorizationUrl: https://mcp.clevertap.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://mcp.clevertap.com/oauth/register
    tokenUrl: https://mcp.clevertap.com/oauth/token
    token_endpoint_auth_methods:
    - none
  - flow: refreshToken
    tokenUrl: https://mcp.clevertap.com/oauth/token
  issuer: https://mcp.clevertap.com/
  name: MCP OAuth 2.1
  source: https://mcp.clevertap.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OpenID Connect scope requesting an identity assertion for the authenticating CleverTap dashboard user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope for the authenticating user's profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope for the authenticating user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Requests a refresh token so the MCP client can keep calling after the access token expires.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: clevertap-scopes
source_filename: clevertap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.clevertap.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  OAuth scopes CleverTap advertises. Scope applies to ONE surface only: the\n  remote MCP server at mcp.clevertap.com. The CleverTap REST API has no OAuth and\n  therefore no scopes — it authenticates with two static headers\n  (X-CleverTap-Account-Id, X-CleverTap-Passcode) with no scoping, expiry or\n  least-privilege model at all. The scopes below were read from the server's own\n  RFC 8414 and RFC 9728 metadata documents, not from documentation: CleverTap\n  publishes no scopes or permissions reference page.\napplies_to:\n  surface: mcp\n  endpoint: https://mcp.clevertap.com/mcp\n  rest_api_uses_oauth: false\nschemes:\n  - name: MCP OAuth 2.1\n    source: https://mcp.clevertap.com/.well-known/oauth-authorization-server\n    issuer: https://mcp.clevertap.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://mcp.clevertap.com/oauth/authorize\n        tokenUrl: https://mcp.clevertap.com/oauth/token\n        registrationUrl: https://mcp.clevertap.com/oauth/register\n        pkce: S256\n        token_endpoint_auth_methods:\n          - none\n      - flow: refreshToken\n        tokenUrl: https://mcp.clevertap.com/oauth/token\nscopes:\n  - scope: openid\n    description: >-\n      Standard OpenID Connect scope requesting an identity assertion for the\n      authenticating CleverTap dashboard user.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/clevertap-oauth-authorization-server.json\n      - well-known/clevertap-oauth-protected-resource.json\n  - scope: profile\n    description: Standard OIDC scope for the authenticating user's profile claims.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/clevertap-oauth-authorization-server.json\n      - well-known/clevertap-oauth-protected-resource.json\n  - scope: email\n    description: Standard\
  \ OIDC scope for the authenticating user's email address.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/clevertap-oauth-authorization-server.json\n      - well-known/clevertap-oauth-protected-resource.json\n  - scope: offline_access\n    description: >-\n      Requests a refresh token so the MCP client can keep calling after the\n      access token expires.\n    flows:\n      - authorizationCode\n      - refreshToken\n    sources:\n      - well-known/clevertap-oauth-authorization-server.json\n      - well-known/clevertap-oauth-protected-resource.json\nanalysis:\n  granularity: identity-only\n  resource_scopes: 0\n  note: >-\n    All four advertised scopes are OIDC identity scopes. There is NO\n    resource-level or action-level scope — nothing like read:profiles or\n    write:campaigns — so an authorized MCP client receives the full authority of\n    the CleverTap user it authenticated as. Least-privilege delegation to an\n    agent is not expressible on this\
  \ surface today.\n  challenge_scope: 'openid profile email'\n  challenge_source: >-\n    WWW-Authenticate header on https://mcp.clevertap.com/mcp — Bearer\n    resource_metadata=\"https://mcp.clevertap.com/.well-known/oauth-protected-resource\",\n    scope=\"openid profile email\"\nx-evidence:\n  fetched: '2026-08-13'\n  urls:\n    - url: https://mcp.clevertap.com/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://mcp.clevertap.com/.well-known/oauth-protected-resource\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/scopes/clevertap-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken
tags:
- Audiences
- Customer Engagement
- Customer Retention
- Marketing Automation
- Mobile Engagement
- Push Notifications
- User Behavior
token_urls:
- https://mcp.clevertap.com/oauth/token
---
