---
api_specs:
- filename: fabric8labs-posts-api-openapi.yml
  format: yaml
  label: Fabric8Labs Posts API
  slug: fabric8labs-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-posts-api-openapi.yml
- filename: fabric8labs-pages-api-openapi.yml
  format: yaml
  label: Fabric8Labs Pages API
  slug: fabric8labs-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-pages-api-openapi.yml
- filename: fabric8labs-media-api-openapi.yml
  format: yaml
  label: Fabric8Labs Media API
  slug: fabric8labs-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-media-api-openapi.yml
- filename: fabric8labs-team-api-openapi.yml
  format: yaml
  label: Fabric8Labs Team API
  slug: fabric8labs-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-team-api-openapi.yml
- filename: fabric8labs-taxonomy-api-openapi.yml
  format: yaml
  label: Fabric8Labs Taxonomy API
  slug: fabric8labs-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-taxonomy-api-openapi.yml
- filename: fabric8labs-search-api-openapi.yml
  format: yaml
  label: Fabric8Labs Search API
  slug: fabric8labs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-search-api-openapi.yml
- filename: fabric8labs-discovery-api-openapi.yml
  format: yaml
  label: Fabric8Labs Discovery API
  slug: fabric8labs-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-discovery-api-openapi.yml
authorization_urls:
- https://www.fabric8labs.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Fabric8Labs Scopes
name_suffix: OAuth Scopes
note: 'Fabric8Labs publishes no scopes reference page — there is no developer portal or documentation host to search. This artifact is therefore built entirely from the machine-readable RFC 8414 and RFC 9728 metadata the site actually serves, both saved verbatim under well-known/. Running 0-working/derive-oauth-scopes.py returned zero, correctly: the seven OpenAPI documents under openapi/ describe the anonymous read surface and declare no oauth2 securityScheme, so the only OAuth surface on this domain is the one the well-known metadata advertises for the MCP endpoint. One scope is published. It was not possible to exercise it — the token endpoint requires a client identity and there is no anonymous path to a grant — so no scope-to-capability mapping is claimed.'
overview: 'Fabric8Labs publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fabric8Labs API on a user''s behalf.


  Tokens are issued from https://www.fabric8labs.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fabric8Labs
provider_slug: fabric8labs
schemes:
- flows:
  - authorizationUrl: https://www.fabric8labs.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    revocationUrl: https://www.fabric8labs.com/oauth/revoke
    tokenUrl: https://www.fabric8labs.com/oauth/token
  issuer: https://www.fabric8labs.com
  name: MCPOAuth
  protected_resource: https://www.fabric8labs.com/wp-json/mcp/mcp-oauth-server
  source: well-known/fabric8labs-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope advertised in scopes_supported by both the authorization-server metadata and the protected-resource metadata. It gates the WordPress MCP Adapter endpoint at /wp-json/mcp/mcp-oauth-server. The provider publishes no description of what the scope grants and no finer-grained scopes; the tool set it unlocks could not be enumerated because tools/list returns HTTP 401 anonymously.
  flows:
  - authorizationCode
  scope: mcp
slug: fabric8labs-scopes
source_filename: fabric8labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.fabric8labs.com/.well-known/oauth-authorization-server\nnote: >-\n  Fabric8Labs publishes no scopes reference page — there is no developer portal or documentation\n  host to search. This artifact is therefore built entirely from the machine-readable RFC 8414 and\n  RFC 9728 metadata the site actually serves, both saved verbatim under well-known/. Running\n  0-working/derive-oauth-scopes.py returned zero, correctly: the seven OpenAPI documents under\n  openapi/ describe the anonymous read surface and declare no oauth2 securityScheme, so the only\n  OAuth surface on this domain is the one the well-known metadata advertises for the MCP endpoint.\n  One scope is published. It was not possible to exercise it — the token endpoint requires a client\n  identity and there is no anonymous path to a grant — so no scope-to-capability mapping is claimed.\nschemes:\n- name: MCPOAuth\n  source: well-known/fabric8labs-oauth-authorization-server.json\n\
  \  issuer: https://www.fabric8labs.com\n  protected_resource: https://www.fabric8labs.com/wp-json/mcp/mcp-oauth-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fabric8labs.com/oauth/authorize\n    tokenUrl: https://www.fabric8labs.com/oauth/token\n    revocationUrl: https://www.fabric8labs.com/oauth/revoke\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: mcp\n  description: >-\n    The single scope advertised in scopes_supported by both the authorization-server metadata and\n    the protected-resource metadata. It gates the WordPress MCP Adapter endpoint at\n    /wp-json/mcp/mcp-oauth-server. The provider publishes no description of what the scope grants\n    and no finer-grained scopes; the tool set it unlocks could not be enumerated because\n    tools/list returns HTTP 401 anonymously.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/fabric8labs-oauth-authorization-server.json\n  - well-known/fabric8labs-oauth-protected-resource.json\n\
  coverage:\n  scopes_published: 1\n  scopes_documented_by_provider: 0\n  granularity: single-scope\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://www.fabric8labs.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.fabric8labs.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://www.fabric8labs.com/wp-json/mcp/mcp-oauth-server\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/scopes/fabric8labs-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Advanced Manufacturing
- Additive Manufacturing
- 3D Printing
- Metal 3D Printing
- Electrochemical Additive Manufacturing
- Thermal Management
- Liquid Cooling
- Data Centers
- Semiconductors
- Electronics
- Aerospace
- Photonics
- Power Electronics
- Hardware
- Content
token_urls:
- https://www.fabric8labs.com/oauth/token
---
