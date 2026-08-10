---
api_specs:
- filename: vestaron-comments-api-openapi.yml
  format: yaml
  label: Vestaron Comments API
  slug: vestaron-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-comments-api-openapi.yml
- filename: vestaron-discovery-api-openapi.yml
  format: yaml
  label: Vestaron Discovery API
  slug: vestaron-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-discovery-api-openapi.yml
- filename: vestaron-media-api-openapi.yml
  format: yaml
  label: Vestaron Media API
  slug: vestaron-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-media-api-openapi.yml
- filename: vestaron-pages-api-openapi.yml
  format: yaml
  label: Vestaron Pages API
  slug: vestaron-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-pages-api-openapi.yml
- filename: vestaron-posts-api-openapi.yml
  format: yaml
  label: Vestaron Posts API
  slug: vestaron-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-posts-api-openapi.yml
- filename: vestaron-search-api-openapi.yml
  format: yaml
  label: Vestaron Search API
  slug: vestaron-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-search-api-openapi.yml
- filename: vestaron-settings-api-openapi.yml
  format: yaml
  label: Vestaron Settings API
  slug: vestaron-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-settings-api-openapi.yml
- filename: vestaron-taxonomy-api-openapi.yml
  format: yaml
  label: Vestaron Taxonomy API
  slug: vestaron-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-taxonomy-api-openapi.yml
- filename: vestaron-users-api-openapi.yml
  format: yaml
  label: Vestaron Users API
  slug: vestaron-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/openapi/vestaron-users-api-openapi.yml
authorization_urls:
- https://vestaron.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Vestaron Scopes
name_suffix: OAuth Scopes
note: Derived from the anonymous RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata that vestaron.com serves for its WordPress MCP endpoint. Vestaron publishes no scope reference page; the single scope below is the complete set the server advertises. Nothing beyond the advertised value is asserted.
overview: 'Vestaron publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vestaron API on a user''s behalf.


  Tokens are issued from https://vestaron.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vestaron
provider_slug: vestaron
schemes:
- flows:
  - authorizationUrl: https://vestaron.com/oauth/authorize
    client_authentication: none
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: required
    refresh_token: true
    revocationUrl: https://vestaron.com/oauth/revoke
    tokenUrl: https://vestaron.com/oauth/token
  issuer: https://vestaron.com
  name: mcp-oauth
  source: well-known/vestaron-oauth-authorization-server.json
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope advertised by the authorization server and by the protected-resource metadata for https://vestaron.com/wp-json/mcp/mcp-oauth-server. Vestaron publishes no further description; the scope's effective permissions could not be determined because tools/list is 401 to anonymous callers.
  flows:
  - authorizationCode
  scope: mcp
slug: vestaron-scopes
source_filename: vestaron-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://vestaron.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the anonymous RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata that vestaron.com serves for its WordPress MCP endpoint. Vestaron\n  publishes no scope reference page; the single scope below is the complete set the server\n  advertises. Nothing beyond the advertised value is asserted.\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  source: well-known/vestaron-oauth-authorization-server.json\n  issuer: https://vestaron.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vestaron.com/oauth/authorize\n    tokenUrl: https://vestaron.com/oauth/token\n    revocationUrl: https://vestaron.com/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    refresh_token: true\n    client_authentication: none\nscopes:\n- scope: mcp\n  description: >-\n    The only scope advertised by\
  \ the authorization server and by the protected-resource metadata\n    for https://vestaron.com/wp-json/mcp/mcp-oauth-server. Vestaron publishes no further\n    description; the scope's effective permissions could not be determined because tools/list is\n    401 to anonymous callers.\n  flows: [authorizationCode]\n  resources: [https://vestaron.com/wp-json/mcp/mcp-oauth-server]\n  sources:\n  - well-known/vestaron-oauth-authorization-server.json\n  - well-known/vestaron-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://vestaron.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://vestaron.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vestaron/refs/heads/main/scopes/vestaron-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Crop Protection
- Bioinsecticides
- Peptides
- Biologicals
- Sustainability
- Pollinator Safety
- Life Sciences
- Content
token_urls:
- https://vestaron.com/oauth/token
---
