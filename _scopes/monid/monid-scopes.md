---
api_specs:
- filename: monid-api-keys-api-openapi.yml
  format: yaml
  label: Monid API Keys API
  slug: monid-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-api-keys-api-openapi.yml
- filename: monid-auth-api-openapi.yml
  format: yaml
  label: Monid Auth API
  slug: monid-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-auth-api-openapi.yml
- filename: monid-controls-api-openapi.yml
  format: yaml
  label: Monid Controls API
  slug: monid-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-controls-api-openapi.yml
- filename: monid-discover-api-openapi.yml
  format: yaml
  label: Monid Discover API
  slug: monid-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-discover-api-openapi.yml
- filename: monid-endpoints-api-openapi.yml
  format: yaml
  label: Monid Endpoints API
  slug: monid-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-endpoints-api-openapi.yml
- filename: monid-inspect-api-openapi.yml
  format: yaml
  label: Monid Inspect API
  slug: monid-inspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-inspect-api-openapi.yml
- filename: monid-public-registry-api-openapi.yml
  format: yaml
  label: Monid Public Registry API
  slug: monid-public-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-public-registry-api-openapi.yml
- filename: monid-resources-api-openapi.yml
  format: yaml
  label: Monid Resources API
  slug: monid-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-resources-api-openapi.yml
- filename: monid-runs-api-openapi.yml
  format: yaml
  label: Monid Runs API
  slug: monid-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-runs-api-openapi.yml
- filename: monid-wallet-api-openapi.yml
  format: yaml
  label: Monid Wallet API
  slug: monid-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-wallet-api-openapi.yml
authorization_urls:
- https://clerk.app.monid.ai/oauth/authorize
description: ''
docs: https://monid.ai/docs/integrations/oauth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Monid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Monid publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Monid API on a user''s behalf.


  Tokens are issued from https://clerk.app.monid.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monid
provider_slug: monid
schemes:
- flows:
  - authorizationUrl: https://clerk.app.monid.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshSupported: true
    revocationUrl: https://clerk.app.monid.ai/oauth/token/revoke
    tokenUrl: https://clerk.app.monid.ai/oauth/token
  name: OAuth2
  provider: Clerk (clerk.app.monid.ai)
  resource: https://api.monid.ai/v1
  type: oauth2
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- user:org:read
scopes:
- description: Required for OIDC. Enables ID tokens.
  flows:
  - authorizationCode
  scope: openid
- description: User's name and profile info.
  flows:
  - authorizationCode
  scope: profile
- description: User's email address.
  flows:
  - authorizationCode
  scope: email
- description: Return a refresh token so you can act while the user is offline.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read the user's organizations and workspaces.
  flows:
  - authorizationCode
  scope: user:org:read
slug: monid-scopes
source_filename: monid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://api.monid.ai/.well-known/openid-configuration\ndocs: https://monid.ai/docs/integrations/oauth.md\nschemes:\n- name: OAuth2\n  type: oauth2\n  provider: Clerk (clerk.app.monid.ai)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.app.monid.ai/oauth/authorize\n    tokenUrl: https://clerk.app.monid.ai/oauth/token\n    revocationUrl: https://clerk.app.monid.ai/oauth/token/revoke\n    refreshSupported: true\n    pkce: S256\n  resource: https://api.monid.ai/v1\nscopes:\n- scope: openid\n  description: Required for OIDC. Enables ID tokens.\n  flows: [authorizationCode]\n- scope: profile\n  description: User's name and profile info.\n  flows: [authorizationCode]\n- scope: email\n  description: User's email address.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Return a refresh token so you can act while the user is offline.\n  flows: [authorizationCode]\n- scope: \"user:org:read\"\
  \n  description: Read the user's organizations and workspaces.\n  flows: [authorizationCode]\nnotes: >-\n  The OpenAPI declares only an HTTP bearer scheme (Monid API key `monid_live_...`\n  or a Clerk-issued JWT). OAuth 2.0 scoped access is documented separately and\n  advertised via the anonymous /.well-known/ discovery documents; agents obtain\n  a user-delegated access token with these scopes to act on the user's own\n  workspace. Authorization requests must include resource=https://api.monid.ai/v1.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/scopes/monid-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Agents
- MCP
- Tools
- Data
- API Marketplace
token_urls:
- https://clerk.app.monid.ai/oauth/token
---
