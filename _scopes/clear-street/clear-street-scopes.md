---
api_specs:
- filename: clear-street-trading-api-openapi.yml
  format: yaml
  label: Clear Street Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-trading-api-openapi.yml
- filename: clear-street-studio-openapi.yml
  format: yaml
  label: Clear Street Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-studio-openapi.yml
- filename: clear-street-legacy-api-swagger.yml
  format: yaml
  label: Clear Street API (Trades and Uploads)
  slug: legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-legacy-api-swagger.yml
authorization_urls:
- https://api.clearstreet.com/oauth/mcp/authorize
- https://auth.clearstreet.io/authorize
description: ''
docs: https://docs.clearstreet.io/studio/docs/oauth2
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clear Street Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securityScheme in either OpenAPI — both specs declare only `BearerAuth` (http/bearer/JWT), which is the token those OAuth flows mint. The OAuth surface below was therefore SEARCHED from the provider's own documentation and from the anonymously-published discovery documents in well-known/, not derived from the specs.
overview: 'Clear Street publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clear Street API on a user''s behalf.


  Tokens are issued from https://auth.clearstreet.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clear Street
provider_slug: clear-street
schemes:
- api: Clear Street Studio API
  credential_creation: 'Studio > Settings > Developer tab > enter an application description > "Create OAuth2 API Credentials" — returns a generated client id and secret. Each application/script should have its own credentials; they inherit the Studio account''s permissions.

    '
  flows:
  - audience: https://api.clearstreet.io
    flow: clientCredentials
    scopes:
    - studio
    tokenUrl: https://auth.clearstreet.io/oauth/token
  issuer: https://auth.clearstreet.io/
  name: Studio OAuth2 (client credentials)
  provider: Auth0
  source: https://docs.clearstreet.io/studio/docs/oauth2
  token_lifetime: 24h
- api: Clear Street MCP Server
  file: well-known/clear-street-mcp-oauth-authorization-server.json
  flows:
  - authorizationUrl: https://api.clearstreet.com/oauth/mcp/authorize
    flow: authorizationCode
    pkce:
    - S256
    scopes:
    - openid
    - offline_access
    tokenUrl: https://auth.clearstreet.io/oauth/token
  issuer: https://api.clearstreet.com/oauth/mcp
  name: Clear Street MCP authorization server
  resource: https://api.clearstreet.com/v1/mcp
  source: https://api.clearstreet.com/oauth/mcp/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
- api: Clear Street application login
  file: well-known/clear-street-openid-configuration.json
  flows:
  - authorizationUrl: https://auth.clearstreet.io/authorize
    flow: authorizationCode
    tokenUrl: https://auth.clearstreet.io/oauth/token
  issuer: https://auth.clearstreet.io/
  name: Auth0 tenant (app login / OIDC)
  source: https://auth.clearstreet.io/.well-known/openid-configuration
scope_count: 5
scope_names:
- studio
- openid
- offline_access
- profile
- email
scopes:
- description: Access to the Clear Street Studio prime-brokerage API.
  flows:
  - clientCredentials
  scope: studio
- description: OIDC — issue an ID token identifying the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the client can renew access without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
- description: OIDC standard claim set — name, nickname, picture, updated_at.
  flows:
  - authorizationCode
  scope: profile
- description: OIDC standard claim — email and email_verified.
  flows:
  - authorizationCode
  scope: email
slug: clear-street-scopes
source_filename: clear-street-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.clearstreet.io/studio/docs/oauth2\ndocs: https://docs.clearstreet.io/studio/docs/oauth2\nnote: >\n  derive-oauth-scopes.py found no oauth2 securityScheme in either OpenAPI — both specs declare\n  only `BearerAuth` (http/bearer/JWT), which is the token those OAuth flows mint. The OAuth\n  surface below was therefore SEARCHED from the provider's own documentation and from the\n  anonymously-published discovery documents in well-known/, not derived from the specs.\nschemes:\n- name: Studio OAuth2 (client credentials)\n  api: Clear Street Studio API\n  issuer: https://auth.clearstreet.io/\n  provider: Auth0\n  source: https://docs.clearstreet.io/studio/docs/oauth2\n  credential_creation: >\n    Studio > Settings > Developer tab > enter an application description > \"Create OAuth2 API\n    Credentials\" — returns a generated client id and secret. Each application/script should have\n    its own credentials; they inherit\
  \ the Studio account's permissions.\n  token_lifetime: 24h\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.clearstreet.io/oauth/token\n    audience: https://api.clearstreet.io\n    scopes: [studio]\n- name: Clear Street MCP authorization server\n  api: Clear Street MCP Server\n  issuer: https://api.clearstreet.com/oauth/mcp\n  source: https://api.clearstreet.com/oauth/mcp/.well-known/oauth-authorization-server\n  file: well-known/clear-street-mcp-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.clearstreet.com/oauth/mcp/authorize\n    tokenUrl: https://auth.clearstreet.io/oauth/token\n    pkce: [S256]\n    scopes: [openid, offline_access]\n  resource: https://api.clearstreet.com/v1/mcp\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n- name: Auth0 tenant (app login / OIDC)\n  api: Clear Street application login\n  issuer: https://auth.clearstreet.io/\n  source: https://auth.clearstreet.io/.well-known/openid-configuration\n\
  \  file: well-known/clear-street-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.clearstreet.io/authorize\n    tokenUrl: https://auth.clearstreet.io/oauth/token\nscopes:\n- scope: studio\n  description: Access to the Clear Street Studio prime-brokerage API.\n  audience: https://api.clearstreet.io\n  flows: [clientCredentials]\n  sources: ['https://docs.clearstreet.io/studio/docs/oauth2']\n- scope: openid\n  description: OIDC — issue an ID token identifying the authenticated subject.\n  flows: [authorizationCode]\n  sources: ['well-known/clear-street-mcp-oauth-protected-resource.json',\n    'well-known/clear-street-openid-configuration.json']\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without re-consent.\n  flows: [authorizationCode]\n  sources: ['well-known/clear-street-mcp-oauth-protected-resource.json',\n    'well-known/clear-street-openid-configuration.json']\n- scope: profile\n \
  \ description: OIDC standard claim set — name, nickname, picture, updated_at.\n  flows: [authorizationCode]\n  sources: ['well-known/clear-street-openid-configuration.json']\n- scope: email\n  description: OIDC standard claim — email and email_verified.\n  flows: [authorizationCode]\n  sources: ['well-known/clear-street-openid-configuration.json']\ntenant_scopes_supported:\n  source: well-known/clear-street-openid-configuration.json\n  note: >\n    The Auth0 tenant advertises the standard OIDC claim scopes below. They govern identity\n    claims on the login flow, not API authorization; the API-level scope is `studio`.\n  values: [openid, profile, offline_access, name, given_name, family_name, nickname, email,\n    email_verified, picture, created_at, identities, phone, address]\ngranularity:\n  per_resource_scopes: false\n  note: >\n    Clear Street does NOT publish per-resource or read/write-split OAuth scopes. Authorization\n    is coarse: a Studio credential inherits the full permission\
  \ set of the Studio account that\n    created it, and the Trading API uses an opaque bearer API key with no scope dimension at\n    all. Least-privilege delegation is not currently expressible.\nx-evidence:\n  fetched: '2026-08-02'\n  sources:\n  - {url: 'https://docs.clearstreet.io/studio/docs/oauth2', http_status: 200}\n  - {url: 'https://auth.clearstreet.io/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://api.clearstreet.com/oauth/mcp/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://api.clearstreet.com/.well-known/oauth-protected-resource/v1/mcp', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/scopes/clear-street-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Company
- Financial Services
- Capital Markets
- Prime Brokerage
- Trading
- Brokerage
- Clearing
- Market Data
- Fintech
- Investing
token_urls:
- https://auth.clearstreet.io/oauth/token
---
