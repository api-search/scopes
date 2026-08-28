---
api_specs:
- filename: redocly-search-api-openapi.yaml
  format: yaml
  label: Redocly Realm Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yaml
- filename: redocly-docs-mcp-openapi.yaml
  format: yaml
  label: Redocly Docs MCP Server
  slug: redocly-docs-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-docs-mcp-openapi.yaml
- filename: redocly-scout-openapi.yaml
  format: yaml
  label: Redocly Scout API
  slug: redocly-scout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-openapi.yaml
- filename: redocly-scout-agent-openapi.yaml
  format: yaml
  label: Redocly Scout Agent API
  slug: redocly-scout-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-agent-openapi.yaml
authorization_urls:
- https://{projectHost}/_mcp/oauth2/auth
description: 'Redocly''s OAuth 2.0 authorization-code flow for the Docs MCP server declares an EMPTY scopes object: authorization is not carried by OAuth scopes at all. Access is decided by Redocly''s RBAC engine — the same teams and roles that gate the portal gate the MCP server and the API descriptions it serves. The nearest thing to a published scope vocabulary is the API-key permission model, which is a UI-selected list of organization and project permissions typed read / write / delete, and Redocly does not publish that list as machine-readable identifiers.'
docs: https://redocly.com/docs/realm/reunite/organization/api-keys#api-key-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Redocly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Redocly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{projectHost}/_mcp/oauth2/token-portal.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Redocly
provider_slug: redocly
schemes:
- flows:
  - authorizationUrl: https://{projectHost}/_mcp/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://{projectHost}/_mcp/oauth2/token-portal
  name: OAuth2
  source: openapi/redocly-docs-mcp-openapi.yaml
scope_count: 0
scope_names: []
scopes: []
slug: redocly-scopes
source_filename: redocly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/redocly-docs-mcp-openapi.yaml OAuth2 flow, plus https://redocly.com/docs/realm/reunite/organization/api-keys\n  (fetched 2026-08-27)\nschemes:\n- name: OAuth2\n  source: openapi/redocly-docs-mcp-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{projectHost}/_mcp/oauth2/auth\n    tokenUrl: https://{projectHost}/_mcp/oauth2/token-portal\nscopes: []\nprovider: Redocly\nproviderId: redocly\ndocs: https://redocly.com/docs/realm/reunite/organization/api-keys#api-key-permissions\ndescription: 'Redocly''s OAuth 2.0 authorization-code flow for the Docs MCP server declares an EMPTY scopes\n  object: authorization is not carried by OAuth scopes at all. Access is decided by Redocly''s RBAC engine\n  — the same teams and roles that gate the portal gate the MCP server and the API descriptions it serves.\n  The nearest thing to a published scope vocabulary is the API-key permission model, which is\
  \ a UI-selected\n  list of organization and project permissions typed read / write / delete, and Redocly does not publish\n  that list as machine-readable identifiers.'\nauthorization_model:\n  type: rbac\n  note: Roles are assigned to teams; API keys either take granular permissions or inherit a team role.\n  feature_flags:\n  - access.rbac.features.mcp\n  - access.rbac.features.aiSearch\n  permission_types:\n  - read\n  - write\n  - delete\nscope_count: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/scopes/redocly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
token_urls:
- https://{projectHost}/_mcp/oauth2/token-portal
---
