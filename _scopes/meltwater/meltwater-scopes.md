---
api_specs:
- filename: meltwater-account-management-api-openapi.yml
  format: yaml
  label: Meltwater Account Management API
  slug: meltwater-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-account-management-api-openapi.yml
- filename: meltwater-bring-your-own-content-byoc-api-openapi.yml
  format: yaml
  label: Meltwater Bring Your Own Content (BYOC) API
  slug: meltwater-bring-your-own-content-byoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-bring-your-own-content-byoc-api-openapi.yml
- filename: meltwater-explore-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Analytics API
  slug: meltwater-explore-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-analytics-api-openapi.yml
- filename: meltwater-explore-assets-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Assets API
  slug: meltwater-explore-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-assets-api-openapi.yml
- filename: meltwater-explore-search-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Search API
  slug: meltwater-explore-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-search-api-openapi.yml
- filename: meltwater-listening-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Listening Analytics API
  slug: meltwater-listening-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-analytics-api-openapi.yml
- filename: meltwater-listening-exports-api-openapi.yml
  format: yaml
  label: Meltwater Listening Exports API
  slug: meltwater-listening-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-exports-api-openapi.yml
- filename: meltwater-listening-search-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search API
  slug: meltwater-listening-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-api-openapi.yml
- filename: meltwater-listening-search-management-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search Management API
  slug: meltwater-listening-search-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-management-api-openapi.yml
- filename: meltwater-listening-streaming-api-openapi.yml
  format: yaml
  label: Meltwater Listening Streaming API
  slug: meltwater-listening-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-streaming-api-openapi.yml
- filename: meltwater-mira-api-api-openapi.yml
  format: yaml
  label: Meltwater Mira API API
  slug: meltwater-mira-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-mira-api-api-openapi.yml
- filename: meltwater-owned-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Owned Analytics API
  slug: meltwater-owned-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-owned-analytics-api-openapi.yml
- filename: meltwater-api-v4-openapi.yml
  format: yaml
  label: Meltwater API v4
  slug: meltwater-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-api-v4-openapi.yml
authorization_urls:
- https://app.meltwater.com/oauth/authorize
description: ''
docs: https://developer.meltwater.com/guides/meltwater-mcp/connecting
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Meltwater Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only an apiKey scheme, so nothing scope-shaped is derivable from the specs. The scopes below were read from Meltwater's own live OAuth discovery documents (RFC 9728 protected-resource metadata on api.meltwater.com, RFC 8414 authorization-server metadata on app.meltwater.com), which are already served even though the MCP connecting guide still describes OAuth 2.0 as "planned for later this year".
overview: 'Meltwater publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meltwater API on a user''s behalf.


  Tokens are issued from https://app.meltwater.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meltwater
provider_slug: meltwater
schemes:
- flows:
  - authorizationUrl: https://app.meltwater.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://app.meltwater.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2
  registration_endpoint: https://app.meltwater.com/oauth/register
  revocation_endpoint: https://app.meltwater.com/oauth/revoke
  source: https://app.meltwater.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
scope_count: 5
scope_names:
- tools:read
- tools:call
- openid
- profile
- email
scopes:
- description: List the MCP tools exposed to the caller's Meltwater package.
  flows:
  - authorizationCode
  scope: tools:read
- description: Invoke an MCP tool against the caller's Meltwater assets and data.
  flows:
  - authorizationCode
  scope: tools:call
- description: OpenID Connect authentication scope advertised by the authorization server.
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim.
  flows:
  - authorizationCode
  scope: email
slug: meltwater-scopes
source_filename: meltwater-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.meltwater.com/.well-known/oauth-protected-resource\ndocs: https://developer.meltwater.com/guides/meltwater-mcp/connecting\nnote: >-\n  The OpenAPI declares only an apiKey scheme, so nothing scope-shaped is derivable from the\n  specs. The scopes below were read from Meltwater's own live OAuth discovery documents\n  (RFC 9728 protected-resource metadata on api.meltwater.com, RFC 8414 authorization-server\n  metadata on app.meltwater.com), which are already served even though the MCP connecting\n  guide still describes OAuth 2.0 as \"planned for later this year\".\nauthorization_server: https://app.meltwater.com\nprotected_resource: https://api.meltwater.com/v2/mcp\nschemes:\n  - name: oauth2\n    source: https://app.meltwater.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.meltwater.com/oauth/authorize\n        tokenUrl: https://app.meltwater.com/oauth/token\n\
  \        pkce: [S256]\n    registration_endpoint: https://app.meltwater.com/oauth/register\n    revocation_endpoint: https://app.meltwater.com/oauth/revoke\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\nscopes:\n  - scope: tools:read\n    description: List the MCP tools exposed to the caller's Meltwater package.\n    flows: [authorizationCode]\n    sources: ['https://api.meltwater.com/.well-known/oauth-protected-resource', 'https://app.meltwater.com/.well-known/oauth-authorization-server']\n  - scope: tools:call\n    description: Invoke an MCP tool against the caller's Meltwater assets and data.\n    flows: [authorizationCode]\n    sources: ['https://api.meltwater.com/.well-known/oauth-protected-resource', 'https://app.meltwater.com/.well-known/oauth-authorization-server']\n  - scope: openid\n    description: OpenID Connect authentication scope advertised by the authorization server.\n    flows: [authorizationCode]\n\
  \    sources: ['https://app.meltwater.com/.well-known/oauth-authorization-server']\n  - scope: profile\n    description: Profile claims.\n    flows: [authorizationCode]\n    sources: ['https://app.meltwater.com/.well-known/oauth-authorization-server']\n  - scope: email\n    description: Email claim.\n    flows: [authorizationCode]\n    sources: ['https://app.meltwater.com/.well-known/oauth-authorization-server']\nx-evidence:\n  - url: https://api.meltwater.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://app.meltwater.com/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/scopes/meltwater-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
token_urls:
- https://app.meltwater.com/oauth/token
---
