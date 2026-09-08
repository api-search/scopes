---
api_specs:
- filename: tray-ai-authentication-api-openapi.yml
  format: yaml
  label: Tray.ai Authentication API
  slug: tray-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentication-api-openapi.yml
- filename: tray-ai-authentications-api-openapi.yml
  format: yaml
  label: Tray.ai Authentications API
  slug: tray-ai-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentications-api-openapi.yml
- filename: tray-ai-call-connector-api-openapi.yml
  format: yaml
  label: Tray.ai Call Connector API
  slug: tray-ai-call-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-call-connector-api-openapi.yml
- filename: tray-ai-connectors-api-openapi.yml
  format: yaml
  label: Tray.ai Connectors API
  slug: tray-ai-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-connectors-api-openapi.yml
- filename: tray-ai-deployments-api-openapi.yml
  format: yaml
  label: Tray.ai Deployments API
  slug: tray-ai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-deployments-api-openapi.yml
- filename: tray-ai-projects-api-openapi.yml
  format: yaml
  label: Tray.ai Projects API
  slug: tray-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-projects-api-openapi.yml
- filename: tray-ai-solution-instances-api-openapi.yml
  format: yaml
  label: Tray.ai Solution Instances API
  slug: tray-ai-solution-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solution-instances-api-openapi.yml
- filename: tray-ai-solutions-api-openapi.yml
  format: yaml
  label: Tray.ai Solutions API
  slug: tray-ai-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solutions-api-openapi.yml
- filename: tray-ai-triggers-api-openapi.yml
  format: yaml
  label: Tray.ai Triggers API
  slug: tray-ai-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-triggers-api-openapi.yml
- filename: tray-ai-users-api-openapi.yml
  format: yaml
  label: Tray.ai Users API
  slug: tray-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-users-api-openapi.yml
- filename: tray-ai-workflows-api-openapi.yml
  format: yaml
  label: Tray.ai Workflows API
  slug: tray-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workflows-api-openapi.yml
- filename: tray-ai-workspaces-api-openapi.yml
  format: yaml
  label: Tray.ai Workspaces API
  slug: tray-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workspaces-api-openapi.yml
authorization_urls: []
description: 'Tray''s OAuth 2.0 scope surface, read verbatim from the RFC 8414 authorization server metadata served at https://api.tray.io/.well-known/oauth-authorization-server (HTTP 200, probed 2026-09-02). These scopes govern the remote MCP server at https://api.tray.io/mcp — Tray''s REST Platform API and GraphQL Embedded API do NOT use OAuth: they take a master or user bearer token and have no scope model. Scope DESCRIPTIONS below are inferred from the scope names and the WWW-Authenticate challenge on the MCP endpoint; Tray publishes no scope reference page.'
docs: https://tray.ai/documentation/platform/artificial-intelligence/agent-gateway/authentication-and-access
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tray Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tray.ai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tray.ai
provider_slug: tray-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tray-ai-scopes
source_filename: tray-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://api.tray.io/.well-known/oauth-authorization-server\ndocs: https://tray.ai/documentation/platform/artificial-intelligence/agent-gateway/authentication-and-access\nprovider: Tray.ai\nproviderId: tray-ai\ndescription: >-\n  Tray's OAuth 2.0 scope surface, read verbatim from the RFC 8414 authorization server metadata\n  served at https://api.tray.io/.well-known/oauth-authorization-server (HTTP 200, probed\n  2026-09-02). These scopes govern the remote MCP server at https://api.tray.io/mcp — Tray's\n  REST Platform API and GraphQL Embedded API do NOT use OAuth: they take a master or user bearer\n  token and have no scope model. Scope DESCRIPTIONS below are inferred from the scope names and\n  the WWW-Authenticate challenge on the MCP endpoint; Tray publishes no scope reference page.\nissuer: https://auth.tray.io\nauthorization_endpoint: https://auth.tray.io/server/oauth2/authorize\ntoken_endpoint: https://auth.tray.io/server/oauth2/token\n\
  registration_endpoint: https://auth.tray.io/server/oauth2/register\nrevocation_endpoint: https://auth.tray.io/server/oauth2/revoke\ngrant_types_supported: [authorization_code, refresh_token]\nresponse_types_supported: [code]\ncode_challenge_methods_supported: [S256]\ntoken_endpoint_auth_methods_supported: [client_secret_basic, none]\ndynamic_client_registration: true\nclient_id_metadata_document_supported: true\nscopes:\n  - name: mcp:list_tools\n    description: >-\n      Discover the tools an MCP server exposes (tools/list). Named in the WWW-Authenticate\n      challenge returned by POST https://api.tray.io/mcp and in the RFC 9728 protected resource\n      metadata for that endpoint.\n    applies_to: https://api.tray.io/mcp\n    verified: probed\n  - name: mcp:call_tools\n    description: >-\n      Invoke a tool on an MCP server (tools/call). These calls act in the caller's Tray\n      organization as the caller and can create, modify and delete projects, workflows and\n      authentications.\n\
  \    applies_to: https://api.tray.io/mcp\n    verified: probed\n  - name: api:full\n    description: >-\n      Full access to the Tray API on behalf of the signed-in user. Advertised in\n      scopes_supported on the authorization server but NOT listed in the MCP resource metadata,\n      so it is a broader grant than the two mcp:* scopes.\n    verified: probed\n    note: >-\n      No Tray documentation page describes this scope. The description above is read from the\n      scope name and its absence from the MCP resource metadata; treat it as unconfirmed.\nnot_applicable:\n  - api: Tray.ai Platform API (REST)\n    reason: >-\n      Bearer master/user token only. Tray's own docs (\"Master and user tokens\") describe token\n      TYPES and RBAC roles, not OAuth scopes.\n  - api: Tray.ai Embedded API (GraphQL)\n    reason: Bearer master/user token only; authority is the token type, not a scope.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/scopes/tray-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automation
- Integration
- iPaaS
- AI Agents
- MCP
- Orchestration
- Workflow Automation
- Connectors
- Agent Gateway
- Embedded Integration
- Enterprise Automation
- Model Context Protocol
token_urls: []
---
