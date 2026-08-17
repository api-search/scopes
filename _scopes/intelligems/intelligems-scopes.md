---
api_specs:
- filename: intelligems-analytics-api-openapi.yml
  format: yaml
  label: Intelligems Analytics API
  slug: intelligems-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-analytics-api-openapi.yml
- filename: intelligems-experiences-api-openapi.yml
  format: yaml
  label: Intelligems Experiences API
  slug: intelligems-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-experiences-api-openapi.yml
- filename: intelligems-holiday-benchmark-api-openapi.yml
  format: yaml
  label: Intelligems Holiday Benchmark API
  slug: intelligems-holiday-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-holiday-benchmark-api-openapi.yml
- filename: intelligems-custom-events-api-openapi.yml
  format: yaml
  label: Intelligems Custom Events API
  slug: intelligems-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/openapi/intelligems-custom-events-api-openapi.yml
authorization_urls:
- https://ai.intelligems.io/oauth/authorize
description: ''
docs: https://docs.intelligems.io/developer-resources/mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Intelligems Scopes
name_suffix: OAuth Scopes
note: Intelligems' OAuth surface is the hosted MCP server, not the External API (which is API-key only — see authentication/intelligems-authentication.yml). The scope set below is read verbatim from the RFC 9728 protected-resource metadata the server publishes anonymously; Intelligems does not document a scopes/permissions reference page, and the metadata advertises exactly one scope. No OpenAPI in this repo declares an oauth2 securityScheme, so nothing here is derived from a spec.
overview: 'Intelligems publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Intelligems API on a user''s behalf.


  Tokens are issued from https://ai.intelligems.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Intelligems
provider_slug: intelligems
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://ai.intelligems.io/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    tokenUrl: https://ai.intelligems.io/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
    - none
  issuer: https://ai.intelligems.io
  name: mcp-oauth2
  registration_endpoint: https://ai.intelligems.io/oauth/register
  source: https://ai.intelligems.io/.well-known/oauth-authorization-server
  surface: https://ai.intelligems.io/mcp
  type: oauth2
scope_count: 1
scope_names:
- member
scopes:
- description: The only scope advertised by the MCP protected-resource metadata. Grants an authenticated organization member's access to that organization's Intelligems data through the MCP tools; per-tool scoping is done with the optional `organization` parameter each tool accepts, not with additional OAuth scopes.
  flows:
  - authorizationCode
  scope: member
slug: intelligems-scopes
source_filename: intelligems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://ai.intelligems.io/.well-known/oauth-protected-resource\ndocs: https://docs.intelligems.io/developer-resources/mcp-server\nnote: >-\n  Intelligems' OAuth surface is the hosted MCP server, not the External API (which is\n  API-key only — see authentication/intelligems-authentication.yml). The scope set below\n  is read verbatim from the RFC 9728 protected-resource metadata the server publishes\n  anonymously; Intelligems does not document a scopes/permissions reference page, and the\n  metadata advertises exactly one scope. No OpenAPI in this repo declares an oauth2\n  securityScheme, so nothing here is derived from a spec.\nschemes:\n  - name: mcp-oauth2\n    type: oauth2\n    surface: https://ai.intelligems.io/mcp\n    source: https://ai.intelligems.io/.well-known/oauth-authorization-server\n    issuer: https://ai.intelligems.io\n    dynamic_client_registration: true\n    registration_endpoint: https://ai.intelligems.io/oauth/register\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://ai.intelligems.io/oauth/authorize\n        tokenUrl: https://ai.intelligems.io/oauth/token\n        pkce: [S256]\n        grant_types: [authorization_code, refresh_token]\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\nscopes:\n  - scope: member\n    description: >-\n      The only scope advertised by the MCP protected-resource metadata. Grants an\n      authenticated organization member's access to that organization's Intelligems\n      data through the MCP tools; per-tool scoping is done with the optional\n      `organization` parameter each tool accepts, not with additional OAuth scopes.\n    flows: [authorizationCode]\n    sources: [https://ai.intelligems.io/.well-known/oauth-protected-resource]\nbearer_methods_supported: [header]\nresource: https://ai.intelligems.io/mcp\nx-evidence:\n  - {url: 'https://ai.intelligems.io/.well-known/oauth-authorization-server', status:\
  \ 200, fetched: '2026-08-13'}\n  - {url: 'https://ai.intelligems.io/.well-known/oauth-protected-resource', status: 200, fetched: '2026-08-13'}\n  - {url: 'https://ai.intelligems.io/mcp', status: 401, fetched: '2026-08-13',\n     note: 'POST tools/list returns WWW-Authenticate: Bearer realm=\"mcp\" — live tool schemas are auth-gated.'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelligems/refs/heads/main/scopes/intelligems-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- A/B Testing
- Ecommerce
- Pricing
- Personalization
- Conversion Rate Optimization
- Shopify
- Analytics
- Experimentation
- MCP
- Webhooks
- Profit Optimization
token_urls:
- https://ai.intelligems.io/oauth/token
---
