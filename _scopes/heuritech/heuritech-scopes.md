---
api_specs:
- filename: heuritech-posts-api-openapi.yml
  format: yaml
  label: Heuritech Posts API
  slug: heuritech-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-posts-api-openapi.yml
- filename: heuritech-pages-api-openapi.yml
  format: yaml
  label: Heuritech Pages API
  slug: heuritech-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-pages-api-openapi.yml
- filename: heuritech-media-api-openapi.yml
  format: yaml
  label: Heuritech Media API
  slug: heuritech-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-media-api-openapi.yml
- filename: heuritech-comments-api-openapi.yml
  format: yaml
  label: Heuritech Comments API
  slug: heuritech-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-comments-api-openapi.yml
- filename: heuritech-taxonomy-api-openapi.yml
  format: yaml
  label: Heuritech Taxonomy API
  slug: heuritech-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-taxonomy-api-openapi.yml
- filename: heuritech-users-api-openapi.yml
  format: yaml
  label: Heuritech Users API
  slug: heuritech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-users-api-openapi.yml
- filename: heuritech-search-api-openapi.yml
  format: yaml
  label: Heuritech Search API
  slug: heuritech-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-search-api-openapi.yml
- filename: heuritech-discovery-api-openapi.yml
  format: yaml
  label: Heuritech Discovery API
  slug: heuritech-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-discovery-api-openapi.yml
authorization_urls:
- https://heuritech.com/oauth/authorize
description: Heuritech's only public OAuth surface is the authorization server advertised on heuritech.com for its remote MCP server. It declares a single coarse scope, `mcp`. There is no published scope or permission reference in any Heuritech documentation, and no Heuritech host publishes an OIDC discovery document. The commercial Heuritech Trend Data API publishes no authentication model at all, so it contributes no scopes; the WordPress REST content surface uses Application Passwords rather than OAuth.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Heuritech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Heuritech publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Heuritech API on a user''s behalf.


  Tokens are issued from https://heuritech.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Heuritech
provider_slug: heuritech
schemes:
- flows:
  - authorizationUrl: https://heuritech.com/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: 'No RFC 7591 registration_endpoint is advertised. The server sets client_id_metadata_document_supported: true, so clients identify themselves with a client-ID metadata document URL rather than pre-registering.'
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://heuritech.com/oauth/revoke
    tokenUrl: https://heuritech.com/oauth/token
  issuer: https://heuritech.com
  name: HeuritechMCPOAuth
  source: https://heuritech.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Heuritech MCP server at https://heuritech.com/wp-json/mcp/mcp-oauth-server. Coarse, single-scope model — the authorization server advertises no finer-grained read/write split, so the scope grants whatever the authenticated WordPress user is permitted to do.
  flows:
  - authorizationCode
  scope: mcp
slug: heuritech-scopes
source_filename: heuritech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://heuritech.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Heuritech's only public OAuth surface is the authorization server advertised on heuritech.com for its\n  remote MCP server. It declares a single coarse scope, `mcp`. There is no published scope or permission\n  reference in any Heuritech documentation, and no Heuritech host publishes an OIDC discovery document.\n  The commercial Heuritech Trend Data API publishes no authentication model at all, so it contributes no\n  scopes; the WordPress REST content surface uses Application Passwords rather than OAuth.\nschemes:\n- name: HeuritechMCPOAuth\n  type: oauth2\n  source: https://heuritech.com/.well-known/oauth-authorization-server\n  issuer: https://heuritech.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://heuritech.com/oauth/authorize\n    tokenUrl: https://heuritech.com/oauth/token\n    revocationUrl: https://heuritech.com/oauth/revoke\n\
  \    pkce: required\n    code_challenge_methods: [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint is advertised. The server sets\n      client_id_metadata_document_supported: true, so clients identify themselves with a client-ID\n      metadata document URL rather than pre-registering.\nscopes:\n- scope: mcp\n  description: >-\n    Access the Heuritech MCP server at https://heuritech.com/wp-json/mcp/mcp-oauth-server. Coarse,\n    single-scope model — the authorization server advertises no finer-grained read/write split, so the\n    scope grants whatever the authenticated WordPress user is permitted to do.\n  flows: [authorizationCode]\n  sources: [https://heuritech.com/.well-known/oauth-authorization-server]\n  protected_resource: https://heuritech.com/wp-json/mcp/mcp-oauth-server\nnot_applicable:\n- surface: Heuritech Trend Data API\n  reason: >-\n    Sales-gated. Heuritech publishes\
  \ no authentication documentation, no OAuth metadata and no\n    specification for the commercial API, so there is no scope surface to record.\n- surface: WordPress REST content API (wp/v2)\n  reason: >-\n    Anonymous for reads; writes use WordPress Application Passwords over HTTP Basic, authorized at\n    https://heuritech.com/wp-admin/authorize-application.php. Not an OAuth surface, so no scopes.\nx-evidence:\n  fetched: '2026-08-17'\n  probes:\n  - url: https://heuritech.com/.well-known/oauth-authorization-server/\n    status: 200\n  - url: https://heuritech.com/.well-known/oauth-protected-resource/\n    status: 200\n  - url: https://heuritech.com/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/scopes/heuritech-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Machine-Learning
- Fashion
- Trend Forecasting
- Demand Forecasting
- Retail
- Luxury
- Market Intelligence
- Consumer Insights
- Social Media Analytics
- Content
token_urls:
- https://heuritech.com/oauth/token
---
