---
api_specs:
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-campaigns-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: hunter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-campaigns-api-openapi.yml
- filename: hunter-combined-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: hunter-combined-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-combined-enrichment-api-openapi.yml
- filename: hunter-company-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: hunter-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-company-enrichment-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-email-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: hunter-email-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-enrichment-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-api-openapi.yml
- filename: hunter-leads-lists-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: hunter-leads-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-lists-api-openapi.yml
authorization_urls:
- https://hunter.io/oauth/authorize
description: Hunter's OAuth surface is not described in the OpenAPI (which declares only API-key and bearer schemes) and is not written up in the API reference. It was discovered by probing RFC 8414 authorization-server metadata on hunter.io, which advertises exactly two coarse scopes. The remote MCP server at mcp.hunter.io publishes RFC 9728 protected-resource metadata naming the same two scopes and hunter.io as its authorization server.
docs: https://hunter.io/api-documentation/v2#authentication
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Hunter Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hunter publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hunter API on a user''s behalf.


  Tokens are issued from https://hunter.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hunter
provider_slug: hunter
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://hunter.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://hunter.io/oauth/token
  - flow: clientCredentials
    tokenUrl: https://hunter.io/oauth/token
  - flow: refreshToken
    tokenUrl: https://hunter.io/oauth/token
  issuer: https://hunter.io
  name: OAuth2
  registration_endpoint: https://hunter.io/oauth/register
  source: https://hunter.io/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access. Granularity is not documented; Hunter publishes no scope reference page, so the mapping from this scope to individual endpoints or MCP tools is not stated anywhere public.
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  scope: read
- description: 'Write access. Same caveat: no published scope-to-operation mapping, so a client cannot tell which of the 100 MCP tools or 25 REST operations a "write" grant actually unlocks.'
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  scope: write
slug: hunter-scopes
source_filename: hunter-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://hunter.io/.well-known/oauth-authorization-server\ndocs: https://hunter.io/api-documentation/v2#authentication\ndescription: >-\n  Hunter's OAuth surface is not described in the OpenAPI (which declares only API-key and bearer\n  schemes) and is not written up in the API reference. It was discovered by probing RFC 8414\n  authorization-server metadata on hunter.io, which advertises exactly two coarse scopes.\n  The remote MCP server at mcp.hunter.io publishes RFC 9728 protected-resource metadata naming\n  the same two scopes and hunter.io as its authorization server.\nschemes:\n- name: OAuth2\n  source: https://hunter.io/.well-known/oauth-authorization-server\n  issuer: https://hunter.io\n  registration_endpoint: https://hunter.io/oauth/register\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  flows:\n  - flow: authorizationCode\n  \
  \  authorizationUrl: https://hunter.io/oauth/authorize\n    tokenUrl: https://hunter.io/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://hunter.io/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://hunter.io/oauth/token\nscopes:\n- scope: read\n  description: >-\n    Read access. Granularity is not documented; Hunter publishes no scope reference page, so the\n    mapping from this scope to individual endpoints or MCP tools is not stated anywhere public.\n  flows: [authorizationCode, clientCredentials, refreshToken]\n  sources: [https://hunter.io/.well-known/oauth-authorization-server, https://mcp.hunter.io/.well-known/oauth-protected-resource]\n- scope: write\n  description: >-\n    Write access. Same caveat: no published scope-to-operation mapping, so a client cannot tell\n    which of the 100 MCP tools or 25 REST operations a \"write\" grant actually unlocks.\n  flows: [authorizationCode, clientCredentials, refreshToken]\n  sources: [https://hunter.io/.well-known/oauth-authorization-server,\
  \ https://mcp.hunter.io/.well-known/oauth-protected-resource]\ngaps:\n- id: no-scope-reference-page\n  detail: Hunter publishes no scopes/permissions reference page; the two scopes are only discoverable from the discovery documents.\n- id: coarse-granularity\n  detail: >-\n    Two scopes cover an API surface that includes destructive bulk deletes, CRM push and sending\n    email sequences. A \"write\" grant is effectively full account control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/scopes/hunter-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
token_urls:
- https://hunter.io/oauth/token
---
