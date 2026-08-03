---
api_specs:
- filename: tricentis-qtest-manager-openapi.yaml
  format: yaml
  label: qTest Manager API v3
  slug: qtest-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-manager-openapi.yaml
- filename: tricentis-qtest-parameters-openapi.yaml
  format: yaml
  label: qTest Parameters API
  slug: qtest-parameters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-parameters-openapi.yaml
- filename: tricentis-qtest-pulse-openapi.yaml
  format: yaml
  label: qTest Pulse API
  slug: qtest-pulse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-pulse-openapi.yaml
- filename: tricentis-qtest-scenario-openapi.yaml
  format: yaml
  label: qTest Scenario API
  slug: qtest-scenario
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-scenario-openapi.yaml
- filename: tricentis-qtest-sessions-openapi.yaml
  format: yaml
  label: qTest Explorer Sessions API
  slug: qtest-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-sessions-openapi.yaml
- filename: tricentis-qtest-data-export-openapi.yaml
  format: yaml
  label: qTest Data Export API
  slug: qtest-data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-data-export-openapi.yaml
- filename: tricentis-qtest-analytics-openapi.json
  format: json
  label: Tricentis Analytics API
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-analytics-openapi.json
- filename: tricentis-neoload-openapi.yaml
  format: yaml
  label: NeoLoad API v3
  slug: neoload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-neoload-openapi.yaml
- filename: tricentis-ttm4j-openapi.json
  format: json
  label: Tricentis Test Management for Jira API
  slug: ttm4j
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-ttm4j-openapi.json
authorization_urls: []
description: ''
docs: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tricentis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tricentis publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tricentis API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tricentis
provider_slug: tricentis
schemes:
- authorization_server: https://<tenant>.my.tricentis.com/_identity
  clients:
  - client_id: MCPServer
    used_by: Tosca Cloud MCP server (via npx mcp-remote, local callback port 56874)
  docs: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm
  flows_documented:
  - flow: authorizationCode
    note: toscactl login opens a browser for PKCE authentication by default.
    pkce: true
  - flow: deviceCode
    note: toscactl login --headless, for CI and headless environments.
  - flow: clientCredentials
    note: non-interactive, via TOSCA_CLIENT_ID and TOSCA_CLIENT_SECRET.
  kind: oauth2
  name: Tosca Cloud identity
  source: docs
scope_count: 1
scope_names:
- tta
scopes:
- description: The scope requested by the Tosca Cloud MCP client (client_id MCPServer). Tricentis publishes the value but no description of what it grants; it appears to cover the Tosca Test Automation surface as a whole rather than a specific resource.
  flows:
  - authorizationCode
  scope: tta
slug: tricentis-scopes
source_filename: tricentis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm\ndocs: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm\nsummary: >-\n  None of the nine harvested Tricentis OpenAPI/Swagger documents declares an oauth2\n  security scheme — every REST surface is header-credential based (bearer token,\n  API key, accountToken, x-access-token, HTTP Basic). The only OAuth surface Tricentis\n  documents is the Tosca Cloud identity service, used by the Tosca Cloud MCP server\n  and the toscactl CLI. Its published scope surface is a single coarse scope; no\n  granular per-resource scope catalogue is published.\noauth_in_specs: false\nschemes:\n- name: Tosca Cloud identity\n  kind: oauth2\n  source: docs\n  docs: https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm\n  authorization_server: https://<tenant>.my.tricentis.com/_identity\n\
  \  clients:\n  - client_id: MCPServer\n    used_by: Tosca Cloud MCP server (via npx mcp-remote, local callback port 56874)\n  flows_documented:\n  - flow: authorizationCode\n    pkce: true\n    note: toscactl login opens a browser for PKCE authentication by default.\n  - flow: deviceCode\n    note: toscactl login --headless, for CI and headless environments.\n  - flow: clientCredentials\n    note: non-interactive, via TOSCA_CLIENT_ID and TOSCA_CLIENT_SECRET.\nscopes:\n- scope: tta\n  description: >-\n    The scope requested by the Tosca Cloud MCP client (client_id MCPServer). Tricentis\n    publishes the value but no description of what it grants; it appears to cover the\n    Tosca Test Automation surface as a whole rather than a specific resource.\n  flows: [authorizationCode]\n  sources: [https://docs.tricentis.com/tosca-cloud/en-us/content/ai_integration/connect_mcp_server.htm]\nkey_auth_products:\n  note: >-\n    These products have no scope surface at all — they authenticate with\
  \ a single\n    credential carrying the caller's full role-based permissions. See\n    authentication/tricentis-authentication.yml.\n  products:\n  - {product: qTest, credential: bearer token from POST /oauth/token, authorization: qTest\n      project and site roles, not scopes}\n  - {product: Tricentis Test Management for Jira, credential: API key in Authorization\n      header, authorization: Jira project permissions}\n  - {product: NeoLoad, credential: accountToken header}\n  - {product: qTest Parameters, credential: x-access-token header}\n  - {product: Tricentis Analytics, credential: HTTP Basic or apikey query parameter}\ngaps:\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is\n  reachable on any anonymous Tricentis host, so the Tosca Cloud scope list could not be\n  read from discovery metadata.\n- qTest exposes an /oauth/token endpoint and an /oauth/status endpoint but declares no\n  oauth2 scheme or scopes in its Swagger; the token is modelled\
  \ as an apiKey header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/scopes/tricentis-scopes.yml
summary_line: 1 scope
tags:
- Company
- Testing
- Test Automation
- Quality Engineering
- Test Management
- Performance Testing
- Continuous Testing
- DevOps
- SAP
- Data Integrity
- Agentic Testing
token_urls: []
---
