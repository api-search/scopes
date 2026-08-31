---
api_specs:
- filename: end-game-threads-api-openapi.yml
  format: yaml
  label: Endgame Threads API
  slug: end-game-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-threads-api-openapi.yml
- filename: end-game-internal-api-openapi.yml
  format: yaml
  label: Endgame Internal API
  slug: end-game-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-internal-api-openapi.yml
- filename: end-game-protected-static-api-openapi.yml
  format: yaml
  label: Endgame Protected Static API
  slug: end-game-protected-static-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-protected-static-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.endgame.io/api-reference/authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: End Game Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Endgame publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Endgame API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Endgame
provider_slug: end-game
schemes:
- authorization_endpoint: https://login.endgame.io/oauth2/authorize
  client_id_metadata_document_supported: true
  code_challenge_methods:
  - S256
  device_authorization_endpoint: https://login.endgame.io/oauth2/device_authorization
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - client_credentials
  introspection_endpoint: https://login.endgame.io/oauth2/introspection
  issuer: https://app.endgame.io
  jwks_uri: https://login.endgame.io/oauth2/jwks
  name: WorkOS OAuth 2.0 (Endgame-provisioned)
  registration_endpoint: https://login.endgame.io/oauth2/register
  source: https://app.endgame.io/.well-known/oauth-authorization-server
  token_endpoint: https://login.endgame.io/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect — request an ID token for the authenticating user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims for the authenticating user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address of the authenticating user.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: end-game-scopes
source_filename: end-game-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.endgame.io/.well-known/oauth-authorization-server\ndocs: https://docs.endgame.io/api-reference/authentication\nraw: well-known/end-game-oauth-authorization-server.json\nsummary: >-\n  Endgame's OAuth surface is authorization-server metadata (RFC 8414) served at\n  app.endgame.io and delegated to WorkOS at login.endgame.io. The advertised scopes\n  are the four OIDC identity scopes only — there are no product-level or\n  resource-level scopes. Authorization to Endgame data is not expressed as OAuth\n  scopes at all: it is decided by the PRINCIPAL behind the credential (a specific\n  user, or the org-wide service identity), as documented on the API authentication\n  page. The REST OpenAPI declares a single http/bearer scheme and no oauth2 scheme,\n  so nothing in the spec carries scopes; this file is derived from the live metadata\n  document rather than from the spec.\nschemes:\n- name: WorkOS OAuth 2.0 (Endgame-provisioned)\n\
  \  source: https://app.endgame.io/.well-known/oauth-authorization-server\n  issuer: https://app.endgame.io\n  authorization_endpoint: https://login.endgame.io/oauth2/authorize\n  token_endpoint: https://login.endgame.io/oauth2/token\n  device_authorization_endpoint: https://login.endgame.io/oauth2/device_authorization\n  introspection_endpoint: https://login.endgame.io/oauth2/introspection\n  registration_endpoint: https://login.endgame.io/oauth2/register\n  jwks_uri: https://login.endgame.io/oauth2/jwks\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - client_credentials\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token for the authenticating user.\n  flows: [authorizationCode, deviceCode]\n  sources:\
  \ [https://app.endgame.io/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Basic profile claims for the authenticating user.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://app.endgame.io/.well-known/oauth-authorization-server]\n- scope: email\n  description: Email address of the authenticating user.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://app.endgame.io/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without re-prompting.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://app.endgame.io/.well-known/oauth-authorization-server]\nconsumers:\n- surface: MCP server\n  endpoint: https://app.endgame.io/api/v1/mcp\n  note: >-\n    The MCP endpoint is a protected resource under this authorization server\n    (well-known/end-game-oauth-protected-resource.json). An unauthenticated\n    tools/list returns 401 with\n    WWW-Authenticate: Bearer\
  \ error=\"invalid_token\", pointing at\n    https://app.endgame.io/api/v1/mcp/.well-known/oauth-protected-resource.\n- surface: Endgame CLI\n  note: endgame auth login runs the authorization_code (browser) or device_code flow.\n- surface: M2M applications\n  note: >-\n    client_credentials grant against https://login.endgame.io/oauth2/token, returning\n    a JWT used as the REST Bearer token. Endgame provisions the WorkOS OAuth client.\nauthorization_model:\n  expressed_as: principal, not scope\n  principals:\n  - {principal: user, credential: 'personal API key (eak_*) or user OAuth token', capabilities: 'create/list/get/rename/delete own threads plus read every org-published thread'}\n  - {principal: org-wide service identity, credential: 'org-wide API key or M2M application token', capabilities: 'read-only — list and fetch org-published threads; every mutation returns 403 FORBIDDEN'}\n  docs: https://docs.endgame.io/api-reference/authentication#scope-and-permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/scopes/end-game-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Sales
- Revenue Intelligence
- Go-To-Market
- Artificial Intelligence
- Agents
- MCP
- Knowledge Graph
- CRM
- Conversation Intelligence
token_urls: []
---
