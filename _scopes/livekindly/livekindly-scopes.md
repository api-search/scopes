---
api_specs:
- filename: livekindly-brands-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Brands API
  slug: livekindly-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-brands-api-openapi.yml
- filename: livekindly-careers-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Careers API
  slug: livekindly-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-careers-api-openapi.yml
- filename: livekindly-comments-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Comments API
  slug: livekindly-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-comments-api-openapi.yml
- filename: livekindly-discovery-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Discovery API
  slug: livekindly-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-discovery-api-openapi.yml
- filename: livekindly-media-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Media API
  slug: livekindly-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-media-api-openapi.yml
- filename: livekindly-pages-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Pages API
  slug: livekindly-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-pages-api-openapi.yml
- filename: livekindly-partners-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Partners API
  slug: livekindly-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-partners-api-openapi.yml
- filename: livekindly-posts-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Posts API
  slug: livekindly-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-posts-api-openapi.yml
- filename: livekindly-search-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Search API
  slug: livekindly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-search-api-openapi.yml
- filename: livekindly-settings-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Settings API
  slug: livekindly-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-settings-api-openapi.yml
- filename: livekindly-taxonomy-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Taxonomy API
  slug: livekindly-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-taxonomy-api-openapi.yml
- filename: livekindly-users-api-openapi.yml
  format: yaml
  label: LIVEKINDLY Users API
  slug: livekindly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/openapi/livekindly-users-api-openapi.yml
authorization_urls:
- https://thelivekindlyco.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Livekindly Scopes
name_suffix: OAuth Scopes
note: 'This OAuth surface exists to authorize the site''s WordPress MCP Adapter, not a product API. The authorization server declares exactly ONE scope — "mcp" — which is the coarse all-or-nothing grant the adapter uses; there is no per-resource or per-ability scope decomposition, so an agent that obtains this scope obtains whatever the granting WordPress user can do through the registered abilities. The wp/v2 content API in openapi/ does NOT use OAuth at all: it is anonymous for reads and WordPress Application Passwords (HTTP Basic) for writes.'
overview: 'LIVEKINDLY publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LIVEKINDLY API on a user''s behalf.


  Tokens are issued from https://thelivekindlyco.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LIVEKINDLY
provider_slug: livekindly
schemes:
- client_id_metadata_document_supported: true
  client_registration:
    dynamic_client_registration: false
    note: 'No registration_endpoint is advertised (RFC 7591 is not offered). Instead the server sets client_id_metadata_document_supported: true — the newer pattern where the client_id is an HTTPS URL resolving to a client-metadata document, which is what the MCP client ecosystem has moved toward.'
  flows:
  - authorizationUrl: https://thelivekindlyco.com/oauth/authorize
    flow: authorizationCode
    pkce:
      code_challenge_methods_supported:
      - S256
      required: true
    refreshUrl: https://thelivekindlyco.com/oauth/token
    tokenUrl: https://thelivekindlyco.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://thelivekindlyco.com
  name: mcp-oauth
  response_types_supported:
  - code
  revocation_endpoint: https://thelivekindlyco.com/oauth/revoke
  source: https://thelivekindlyco.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope the authorization server advertises. Grants a bearer token accepted by the MCP protected resource at /wp-json/mcp/mcp-oauth-server. Scope semantics are not published; the tool set it unlocks could not be enumerated because tools/list is authentication-gated.
  flows:
  - authorizationCode
  scope: mcp
slug: livekindly-scopes
source_filename: livekindly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://thelivekindlyco.com/.well-known/oauth-authorization-server\nalso_source: https://thelivekindlyco.com/.well-known/oauth-protected-resource\ndocs: null\ndocs_note: >-\n  LIVEKINDLY publishes no developer documentation of any kind, so there is no scopes or\n  permissions reference page to search. Everything below is taken verbatim from the two live\n  discovery documents saved in well-known/. Nothing is inferred.\nnote: >-\n  This OAuth surface exists to authorize the site's WordPress MCP Adapter, not a product API. The\n  authorization server declares exactly ONE scope — \"mcp\" — which is the coarse all-or-nothing\n  grant the adapter uses; there is no per-resource or per-ability scope decomposition, so an\n  agent that obtains this scope obtains whatever the granting WordPress user can do through the\n  registered abilities. The wp/v2 content API in openapi/ does NOT use OAuth at all: it is\n  anonymous for reads and\
  \ WordPress Application Passwords (HTTP Basic) for writes.\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  source: https://thelivekindlyco.com/.well-known/oauth-authorization-server\n  issuer: https://thelivekindlyco.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thelivekindlyco.com/oauth/authorize\n    tokenUrl: https://thelivekindlyco.com/oauth/token\n    refreshUrl: https://thelivekindlyco.com/oauth/token\n    pkce:\n      required: true\n      code_challenge_methods_supported: [S256]\n  revocation_endpoint: https://thelivekindlyco.com/oauth/revoke\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  client_registration:\n    dynamic_client_registration: false\n    note: >-\n      No registration_endpoint is advertised (RFC 7591 is not offered). Instead the server sets\n      client_id_metadata_document_supported:\
  \ true — the newer pattern where the client_id is an\n      HTTPS URL resolving to a client-metadata document, which is what the MCP client ecosystem\n      has moved toward.\nscopes:\n- scope: mcp\n  description: >-\n    The only scope the authorization server advertises. Grants a bearer token accepted by the MCP\n    protected resource at /wp-json/mcp/mcp-oauth-server. Scope semantics are not published; the\n    tool set it unlocks could not be enumerated because tools/list is authentication-gated.\n  flows: [authorizationCode]\n  sources:\n  - https://thelivekindlyco.com/.well-known/oauth-authorization-server\n  - https://thelivekindlyco.com/.well-known/oauth-protected-resource\nprotected_resources:\n- resource: https://thelivekindlyco.com/wp-json/mcp/mcp-oauth-server\n  authorization_servers: [https://thelivekindlyco.com]\n  bearer_methods_supported: [header]\n  scopes_supported: [mcp]\n  spec: RFC 9728\nx-evidence:\n  fetched: '2026-08-04'\n  authorization_server_metadata:\n    url:\
  \ https://thelivekindlyco.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n    file: ../well-known/livekindly-oauth-authorization-server.json\n  protected_resource_metadata:\n    url: https://thelivekindlyco.com/.well-known/oauth-protected-resource\n    http_status: 200\n    content_type: application/json\n    file: ../well-known/livekindly-oauth-protected-resource.json\n  anonymous_token_probe: >-\n    Not attempted. Obtaining a token requires an interactive authorization grant from a\n    LIVEKINDLY WordPress account; no credential of any kind was used in building this profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livekindly/refs/heads/main/scopes/livekindly-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Food and Beverage
- Plant-Based
- Alternative Protein
- Consumer Packaged Goods
- Sustainability
- Manufacturing
- Retail
- Content
- Newsroom
token_urls:
- https://thelivekindlyco.com/oauth/token
---
