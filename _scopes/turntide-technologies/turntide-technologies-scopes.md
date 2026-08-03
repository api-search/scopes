---
api_specs:
- filename: turntide-technologies-wordpress-rest-openapi.yml
  format: yaml
  label: Turntide WordPress REST API
  slug: turntide-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turntide-technologies/refs/heads/main/openapi/turntide-technologies-wordpress-rest-openapi.yml
authorization_urls:
- https://turntide.com/oauth/authorize
description: ''
docs: https://turntide.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Turntide Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Turntide Technologies publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Turntide Technologies API on a user''s behalf.


  Tokens are issued from https://turntide.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Turntide Technologies
provider_slug: turntide-technologies
schemes:
- description: OAuth 2.1 authorization server advertised at https://turntide.com/.well-known/oauth-authorization-server (PKCE S256, scope 'mcp'); protects the MCP endpoint declared at https://turntide.com/.well-known/oauth-protected-resource
  flows:
  - authorizationUrl: https://turntide.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://turntide.com/oauth/token
  name: mcpOAuth2
  source: openapi/turntide-technologies-wordpress-rest-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Turntide MCP server
  flows:
  - authorizationCode
  scope: mcp
slug: turntide-technologies-scopes
source_filename: turntide-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://turntide.com/.well-known/oauth-authorization-server\ndocs: https://turntide.com/.well-known/oauth-protected-resource\nscope_note: >-\n  The single scope \"mcp\" is not inferred — it is published verbatim as scopes_supported in the\n  live RFC 8414 authorization server metadata and repeated in the RFC 9728 protected resource\n  metadata. Turntide publishes no human-readable scope reference page; there is no broader\n  permission model, because the only OAuth-protected resource is the MCP endpoint.\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - {url: 'https://turntide.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://turntide.com/.well-known/oauth-protected-resource', http_status: 200}\n  files:\n  - well-known/turntide-technologies-oauth-authorization-server.json\n  - well-known/turntide-technologies-oauth-protected-resource.json\nschemes:\n- name: mcpOAuth2\n  source: openapi/turntide-technologies-wordpress-rest-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://turntide.com/oauth/authorize\n    tokenUrl: https://turntide.com/oauth/token\n  description: OAuth 2.1 authorization server advertised at https://turntide.com/.well-known/oauth-authorization-server\n    (PKCE S256, scope 'mcp'); protects the MCP endpoint declared at https://turntide.com/.well-known/oauth-protected-resource\nscopes:\n- scope: mcp\n  description: Access the Turntide MCP server\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/turntide-technologies-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turntide-technologies/refs/heads/main/scopes/turntide-technologies-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Electrification
- Electric Motors
- Power Electronics
- Energy Storage
- Thermal Management
- Industrial Equipment
- Manufacturing
- Sustainability
- Building Automation
- Content Management
token_urls:
- https://turntide.com/oauth/token
---
