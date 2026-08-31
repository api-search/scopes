---
api_specs:
- filename: clozd-programs-api-openapi.yml
  format: yaml
  label: Clozd /programs API
  slug: clozd-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-api-openapi.yml
- filename: clozd-programs-program-id-competitors-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/competitors API
  slug: clozd-programs-program-id-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-competitors-api-openapi.yml
- filename: clozd-programs-program-id-deals-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals API
  slug: clozd-programs-program-id-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-api-openapi.yml
- filename: clozd-programs-program-id-deals-deal-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/:deal ID API
  slug: clozd-programs-program-id-deals-deal-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-deal-id-api-openapi.yml
- filename: clozd-programs-program-id-deals-import-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/deals/import API
  slug: clozd-programs-program-id-deals-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-deals-import-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints API
  slug: clozd-programs-program-id-touchpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-api-openapi.yml
- filename: clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
  format: yaml
  label: Clozd /programs/:program Id/touchpoints/:touchpoint ID API
  slug: clozd-programs-program-id-touchpoints-touchpoint-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/openapi/clozd-programs-program-id-touchpoints-touchpoint-id-api-openapi.yml
authorization_urls:
- https://oauth.clozd.com/authorize
description: ''
docs: https://help.clozd.com/hc/en-us/articles/49656607624987-Connecting-to-Clozd-via-MCP
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Clozd Scopes
name_suffix: OAuth Scopes
note: Clozd's OpenAPI Data API (v1/v2/v3) declares no oauth2 security scheme — it is API-key only — so this artifact is derived entirely from the OAuth 2.0 authorization server that protects the Clozd MCP server. Clozd publishes no per-tool or per-resource scope reference beyond the scopes_supported list below; authorization inside the platform is enforced by role-based access control on the authenticated user and by the program scoping an admin grants, not by fine-grained OAuth scopes.
overview: 'Clozd publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clozd API on a user''s behalf.


  Tokens are issued from https://oauth.clozd.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clozd
provider_slug: clozd
schemes:
- endpoints:
    dynamic_client_registration: https://oauth.clozd.com/register
    introspection: https://oauth.clozd.com/introspect
    jwks: https://oauth.clozd.com/.well-known/jwks.json
    revocation: https://oauth.clozd.com/revoke
    userinfo: https://oauth.clozd.com/userinfo
  flows:
  - authorizationUrl: https://oauth.clozd.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://oauth.clozd.com/token
  - flow: clientCredentials
    tokenUrl: https://oauth.clozd.com/token
  - flow: refreshToken
    tokenUrl: https://oauth.clozd.com/token
  issuer: https://oauth.clozd.com
  name: Clozd OAuth 2.0 / OIDC
  source: https://oauth.clozd.com/.well-known/oauth-authorization-server
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- api
scopes:
- description: OpenID Connect authentication — issues an ID token identifying the Clozd user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the authenticated user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token so an MCP client can keep the connection alive without re-prompting the user for interactive login.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
- description: Access to the Clozd API/MCP resource. Single coarse-grained resource scope — the data a token can reach is determined by the user's platform role and the programs an admin has scoped to them, not by the scope string.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api
slug: clozd-scopes
source_filename: clozd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://oauth.clozd.com/.well-known/oauth-authorization-server\ndocs: https://help.clozd.com/hc/en-us/articles/49656607624987-Connecting-to-Clozd-via-MCP\nnote: >-\n  Clozd's OpenAPI Data API (v1/v2/v3) declares no oauth2 security scheme — it is API-key only — so this\n  artifact is derived entirely from the OAuth 2.0 authorization server that protects the Clozd MCP server.\n  Clozd publishes no per-tool or per-resource scope reference beyond the scopes_supported list below;\n  authorization inside the platform is enforced by role-based access control on the authenticated user and\n  by the program scoping an admin grants, not by fine-grained OAuth scopes.\napplies_to:\n  api: Clozd MCP Server\n  resource: https://mcp.clozd.com/mcp\nschemes:\n- name: Clozd OAuth 2.0 / OIDC\n  issuer: https://oauth.clozd.com\n  source: https://oauth.clozd.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n   \
  \ authorizationUrl: https://oauth.clozd.com/authorize\n    tokenUrl: https://oauth.clozd.com/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://oauth.clozd.com/token\n  - flow: refreshToken\n    tokenUrl: https://oauth.clozd.com/token\n  endpoints:\n    userinfo: https://oauth.clozd.com/userinfo\n    revocation: https://oauth.clozd.com/revoke\n    introspection: https://oauth.clozd.com/introspect\n    jwks: https://oauth.clozd.com/.well-known/jwks.json\n    dynamic_client_registration: https://oauth.clozd.com/register\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issues an ID token identifying the Clozd user.\n  standard: OpenID Connect Core 1.0\n  flows:\n  - authorizationCode\n  sources:\n  - https://oauth.clozd.com/.well-known/openid-configuration\n- scope: profile\n  description: Access to the authenticated user's basic profile claims.\n  standard: OpenID Connect Core 1.0\n  flows:\n  - authorizationCode\n  sources:\n  - https://oauth.clozd.com/.well-known/openid-configuration\n\
  - scope: email\n  description: Access to the authenticated user's email address claim.\n  standard: OpenID Connect Core 1.0\n  flows:\n  - authorizationCode\n  sources:\n  - https://oauth.clozd.com/.well-known/openid-configuration\n- scope: offline_access\n  description: >-\n    Issues a refresh token so an MCP client can keep the connection alive without re-prompting the user for\n    interactive login.\n  standard: OpenID Connect Core 1.0\n  flows:\n  - authorizationCode\n  - refreshToken\n  sources:\n  - https://oauth.clozd.com/.well-known/openid-configuration\n- scope: api\n  description: >-\n    Access to the Clozd API/MCP resource. Single coarse-grained resource scope — the data a token can reach\n    is determined by the user's platform role and the programs an admin has scoped to them, not by the\n    scope string.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://oauth.clozd.com/.well-known/oauth-authorization-server\n  - https://mcp.clozd.com/.well-known/oauth-protected-resource/mcp\n\
  granularity:\n  model: coarse\n  per_tool_scopes: false\n  per_resource_scopes: false\n  read_write_split: false\n  note: >-\n    A single `api` scope covers the whole MCP surface. Because every published MCP tool is read-only, the\n    absence of a read/write split does not currently expose write operations to agents, but it also gives a\n    consuming agent no way to request least privilege.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://oauth.clozd.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - url: https://oauth.clozd.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - url: https://mcp.clozd.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clozd/refs/heads/main/scopes/clozd-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- win-loss-analysis
- customer-feedback
- decision-intelligence
- sales-intelligence
- market-research
- Competitive Intelligence
- voice-of-customer
- revenue-intelligence
- saas
- MCP
- agent-native
token_urls:
- https://oauth.clozd.com/token
---
