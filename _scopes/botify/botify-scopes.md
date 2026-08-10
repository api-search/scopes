---
api_specs:
- filename: botify-analysis-api-openapi.yml
  format: yaml
  label: Botify Analysis API
  slug: botify-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-analysis-api-openapi.yml
- filename: botify-collections-api-openapi.yml
  format: yaml
  label: Botify Collections API
  slug: botify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-collections-api-openapi.yml
- filename: botify-datasource-api-openapi.yml
  format: yaml
  label: Botify Datasource API
  slug: botify-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-datasource-api-openapi.yml
- filename: botify-job-api-openapi.yml
  format: yaml
  label: Botify Job API
  slug: botify-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-job-api-openapi.yml
- filename: botify-keywordsgroups-api-openapi.yml
  format: yaml
  label: Botify Keywords Groups API
  slug: botify-keywordsgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-keywordsgroups-api-openapi.yml
- filename: botify-project-api-openapi.yml
  format: yaml
  label: Botify Project API
  slug: botify-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-project-api-openapi.yml
- filename: botify-projectquery-api-openapi.yml
  format: yaml
  label: Botify Project Query API
  slug: botify-projectquery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-projectquery-api-openapi.yml
- filename: botify-user-api-openapi.yml
  format: yaml
  label: Botify User API
  slug: botify-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-user-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.botify.com/docs/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Botify Scopes
name_suffix: OAuth Scopes
note: 'Botify''s OAuth surface exists only for its MCP server. The REST API at api.botify.com/v1 is not OAuth-based — it uses a single per-user API token in the Authorization header with no scope concept at all (see authentication/botify-authentication.yml). The authorization server at app.botify.com advertises exactly one scope, and it is coarse: a single read-write grant over the whole MCP surface. There is no read-only variant, no per-product (SiteCrawler / LogAnalyzer / RealKeywords) split, and no per-project scoping in the published metadata.'
overview: 'Botify uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Botify
provider_slug: botify
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: botify-scopes
source_filename: botify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://app.botify.com/.well-known/oauth-authorization-server\ndocs: https://developers.botify.com/docs/getting-started\nnote: >-\n  Botify's OAuth surface exists only for its MCP server. The REST API at api.botify.com/v1 is not OAuth-based —\n  it uses a single per-user API token in the Authorization header with no scope concept at all\n  (see authentication/botify-authentication.yml). The authorization server at app.botify.com advertises exactly\n  one scope, and it is coarse: a single read-write grant over the whole MCP surface. There is no read-only\n  variant, no per-product (SiteCrawler / LogAnalyzer / RealKeywords) split, and no per-project scoping in the\n  published metadata.\nauthorization_server: https://app.botify.com/\nprotected_resources:\n- resource: https://mcp.botify.com/\n  resource_name: Botify Agents MCP\n  scopes_supported:\n  - mcp_read_write\nscopes:\n- name: mcp_read_write\n  description: >-\n    The only\
  \ scope advertised by the Botify authorization server. Granted to an MCP client after the\n    authorization-code + PKCE flow; combined read and write access to the Botify Agents MCP surface.\n    Botify publishes no further description of what it covers.\n  read_only: false\n  source: https://app.botify.com/.well-known/oauth-authorization-server\nflows:\n  authorization_code:\n    authorization_endpoint: https://app.botify.com/oauth/authorize\n    token_endpoint: https://app.botify.com/oauth/token/\n    pkce_methods:\n    - S256\n  refresh_token: true\nendpoints:\n  registration: https://app.botify.com/oauth/register/\n  revocation: https://app.botify.com/oauth/revoke/\n  introspection: https://app.botify.com/oauth/introspect/\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- none\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n  - url: https://app.botify.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n\
  \  - url: https://mcp.botify.com/.well-known/oauth-protected-resource\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/scopes/botify-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- seo
- organic-search
- search-engine-optimization
- web-crawling
- log-analysis
- search-console
- marketing-analytics
- ai-search
- data-export
- mcp
- agent-native
token_urls: []
---
