---
api_specs:
- filename: doit-openapi-original.yml
  format: yaml
  label: DoiT API
  slug: doit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/openapi/doit-openapi-original.yml
authorization_urls:
- https://console.doit.com/sign-in/oauth
description: ''
docs: https://developer.doit.com/docs/start
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Doit Scopes
name_suffix: OAuth Scopes
note: DoiT runs two OAuth surfaces from one authorization server. The DoiT Platform API declares a single coarse scope (dci — "Access All Data"), and the MCP resource declares three of its own. Neither surface publishes a fine-grained read/write scope taxonomy; authorization is enforced by the DoiT role or service-account permissions behind the token, not by scope. An agent cannot request least privilege through scopes here.
overview: 'DoiT publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DoiT API on a user''s behalf.


  Tokens are issued from https://console.doit.com/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DoiT
provider_slug: doit
schemes:
- flows:
  - authorizationUrl: https://console.doit.com/sign-in/oauth
    flow: authorizationCode
    tokenUrl: https://console.doit.com/api/auth/token
  name: oauth2
  source: openapi/doit-openapi-original.yml
- authorization_servers:
  - https://console.doit.com
  bearer_methods_supported:
  - header
  name: mcp-oauth
  resource: https://mcp.doit.com
  source: https://mcp.doit.com/.well-known/oauth-protected-resource
scope_count: 4
scope_names:
- dci
- mcp:tools
- mcp:resources
- offline_access
scopes:
- description: Access All Data
  flows:
  - authorizationCode
  scope: dci
- description: Invoke tools exposed by the DoiT MCP server
  flows: []
  scope: mcp:tools
- description: Read resources exposed by the DoiT MCP server
  flows: []
  scope: mcp:resources
- description: Obtain a refresh token for long-lived access without re-authorization
  flows: []
  scope: offline_access
slug: doit-scopes
source_filename: doit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/doit-openapi-original.yml + https://mcp.doit.com/.well-known/oauth-protected-resource\ndocs: https://developer.doit.com/docs/start\nnote: DoiT runs two OAuth surfaces from one authorization server. The DoiT Platform API\n  declares a single coarse scope (dci — \"Access All Data\"), and the MCP resource declares\n  three of its own. Neither surface publishes a fine-grained read/write scope taxonomy;\n  authorization is enforced by the DoiT role or service-account permissions behind the\n  token, not by scope. An agent cannot request least privilege through scopes here.\nauthorization_server:\n  issuer: https://console.doit.com\n  metadata: https://console.doit.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://console.doit.com/oauth/authorize\n  token_endpoint: https://console.doit.com/api/auth/token\n  registration_endpoint: https://console.doit.com/api/oauth/register\n  revocation_endpoint:\
  \ https://console.doit.com/api/oauth/revoke\n  jwks_uri: https://console.doit.com/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  pkce: S256\n  resource_indicators_supported: true\nschemes:\n- name: oauth2\n  source: openapi/doit-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.doit.com/sign-in/oauth\n    tokenUrl: https://console.doit.com/api/auth/token\n- name: mcp-oauth\n  source: https://mcp.doit.com/.well-known/oauth-protected-resource\n  resource: https://mcp.doit.com\n  authorization_servers:\n  - https://console.doit.com\n  bearer_methods_supported:\n  - header\nscopes:\n- scope: dci\n  description: Access All Data\n  surface: DoiT Platform API (https://api.doit.com)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/doit-openapi-original.yml\n  note: The only scope the API contract declares. It is all-or-nothing — there is no\n    read-only\
  \ variant.\n- scope: mcp:tools\n  description: Invoke tools exposed by the DoiT MCP server\n  surface: DoiT MCP server (https://mcp.doit.com)\n  sources:\n  - https://mcp.doit.com/.well-known/oauth-protected-resource\n- scope: mcp:resources\n  description: Read resources exposed by the DoiT MCP server\n  surface: DoiT MCP server (https://mcp.doit.com)\n  sources:\n  - https://mcp.doit.com/.well-known/oauth-protected-resource\n- scope: offline_access\n  description: Obtain a refresh token for long-lived access without re-authorization\n  surface: DoiT MCP server (https://mcp.doit.com)\n  sources:\n  - https://mcp.doit.com/.well-known/oauth-protected-resource\npermission_model:\n  mechanism: role-based, enforced per operation behind the token\n  detail: Personal API tokens inherit the creating user's role permissions and narrow\n    if that role changes. Service-account tokens use the service account's current permissions,\n    with changes effective immediately and removed permissions producing\
  \ 403 on affected\n    endpoints. Each API operation enforces its own permissions independently of scope.\n  docs: https://developer.doit.com/docs/start\nx-evidence:\n- url: https://api.doit.com/openapi.yaml\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://mcp.doit.com/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://console.doit.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://developer.doit.com/docs/start\n  http_status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/scopes/doit-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud Intelligence
- Cost Optimization
- Multicloud
- Kubernetes
- Analytics
- MCP
- Artificial Intelligence
token_urls:
- https://console.doit.com/api/auth/token
---
