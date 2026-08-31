---
api_specs:
- filename: scimar-comments-api-openapi.yml
  format: yaml
  label: Scimar Comments API
  slug: scimar-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-comments-api-openapi.yml
- filename: scimar-discovery-api-openapi.yml
  format: yaml
  label: Scimar Discovery API
  slug: scimar-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-discovery-api-openapi.yml
- filename: scimar-media-api-openapi.yml
  format: yaml
  label: Scimar Media API
  slug: scimar-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-media-api-openapi.yml
- filename: scimar-pages-api-openapi.yml
  format: yaml
  label: Scimar Pages API
  slug: scimar-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-pages-api-openapi.yml
- filename: scimar-posts-api-openapi.yml
  format: yaml
  label: Scimar Posts API
  slug: scimar-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-posts-api-openapi.yml
- filename: scimar-search-api-openapi.yml
  format: yaml
  label: Scimar Search API
  slug: scimar-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-search-api-openapi.yml
- filename: scimar-settings-api-openapi.yml
  format: yaml
  label: Scimar Settings API
  slug: scimar-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-settings-api-openapi.yml
- filename: scimar-taxonomy-api-openapi.yml
  format: yaml
  label: Scimar Taxonomy API
  slug: scimar-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-taxonomy-api-openapi.yml
- filename: scimar-users-api-openapi.yml
  format: yaml
  label: Scimar Users API
  slug: scimar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Scimar Scopes
name_suffix: OAuth Scopes
note: 'The OpenAPI derived for the wp/v2 content surface declares no oauth2 securityScheme — that surface uses WordPress Application Passwords over HTTP Basic and has no scope model. The OAuth surface on this domain belongs to the WordPress MCP Adapter, and its scope inventory is published, machine readable and anonymous: both RFC 8414 and RFC 9728 metadata documents return 200 and both declare the same single scope. That is the whole scope surface — one scope, taken verbatim from the provider''s own documents. Nothing is expanded, split or inferred.'
overview: 'Scimar uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scimar
provider_slug: scimar
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: scimar-scopes
source_filename: scimar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://scimar.ca/.well-known/oauth-authorization-server + https://scimar.ca/.well-known/oauth-protected-resource\ndocs: null\napplies_to: scimar:mcp\nnote: >-\n  The OpenAPI derived for the wp/v2 content surface declares no oauth2 securityScheme — that surface\n  uses WordPress Application Passwords over HTTP Basic and has no scope model. The OAuth surface on\n  this domain belongs to the WordPress MCP Adapter, and its scope inventory is published, machine\n  readable and anonymous: both RFC 8414 and RFC 9728 metadata documents return 200 and both declare\n  the same single scope. That is the whole scope surface — one scope, taken verbatim from the\n  provider's own documents. Nothing is expanded, split or inferred.\nauthorization_server:\n  issuer: https://scimar.ca\n  authorization_endpoint: https://scimar.ca/oauth/authorize\n  token_endpoint: https://scimar.ca/oauth/token\n  revocation_endpoint: https://scimar.ca/oauth/revoke\n\
  \  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\nprotected_resource:\n  resource: https://scimar.ca/wp-json/mcp/mcp-oauth-server\n  authorization_servers: [https://scimar.ca]\n  bearer_methods_supported: [header]\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The only scope advertised. Declared in scopes_supported of both the authorization-server metadata\n    and the protected-resource metadata. Scimar publishes no scope reference page and no description\n    of what the scope grants, so its effective permissions are unknown — the WordPress MCP Adapter\n    projects the site's registered wp-abilities as tools, and the abilities registry is itself gated\n    (GET /wp-json/wp-abilities/v1/abilities -> 401), so the grant cannot be\
  \ enumerated anonymously.\n  grants: unknown\n  source: /.well-known/oauth-authorization-server\n  read_write: unknown\ngaps:\n- >-\n  No scope reference or permissions documentation exists anywhere on scimar.ca. A single coarse \"mcp\"\n  scope is all the authorization surface an integrator can see, and it is not decomposed by capability\n  or by read-versus-write.\n- >-\n  token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients only, with PKCE S256 required.\n  There is no client-secret path.\nevidence:\n- {url: 'https://scimar.ca/.well-known/oauth-authorization-server', status: 200}\n- {url: 'https://scimar.ca/.well-known/oauth-protected-resource', status: 200}\n- {url: 'https://scimar.ca/wp-json/wp-abilities/v1/abilities', status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/scopes/scimar-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Diabetes
- Diagnostics
- Clinical Trials
- Health
- Nutrition
- Research
- Canada
- Content
token_urls: []
---
