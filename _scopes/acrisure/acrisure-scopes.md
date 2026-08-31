---
authorization_urls:
- https://api.acrisure.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Acrisure Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Acrisure publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Acrisure API on a user''s behalf.


  Tokens are issued from https://api.acrisure.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acrisure
provider_slug: acrisure
schemes:
- flows:
  - authorizationUrl: https://api.acrisure.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.acrisure.com/oauth/token
  issuer: https://api.acrisure.com
  name: AcrisureOAuth2
  source: https://api.acrisure.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- api://bc250bc0-7689-4f21-b164-72a6b57c273b/mcp_user
- offline_access
scopes:
- description: Microsoft Entra ID application scope granting a user-delegated session against the Acrisure MCP server at https://api.acrisure.com/v1/mcp. Description inferred from the scope name; Acrisure publishes no scope reference.
  flows:
  - authorizationCode
  scope: api://bc250bc0-7689-4f21-b164-72a6b57c273b/mcp_user
- description: Standard OIDC scope. Permits issuance of a refresh token so an agent session can outlive the initial access token.
  flows:
  - authorizationCode
  scope: offline_access
slug: acrisure-scopes
source_filename: acrisure-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://api.acrisure.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Acrisure publishes no scopes or permissions reference page. Every scope below is verbatim\n  from the `scopes_supported` array of the RFC 8414 authorization-server metadata; the\n  descriptions are our reading of the scope names, not Acrisure text.\nschemes:\n- name: AcrisureOAuth2\n  source: https://api.acrisure.com/.well-known/oauth-authorization-server\n  issuer: https://api.acrisure.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.acrisure.com/oauth/authorize\n    tokenUrl: https://api.acrisure.com/oauth/token\nscopes:\n- scope: api://bc250bc0-7689-4f21-b164-72a6b57c273b/mcp_user\n  description: >-\n    Microsoft Entra ID application scope granting a user-delegated session against the\n    Acrisure MCP server at https://api.acrisure.com/v1/mcp. Description inferred from the\n    scope name; Acrisure publishes\
  \ no scope reference.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.acrisure.com/.well-known/oauth-authorization-server\n  resource_app_id: bc250bc0-7689-4f21-b164-72a6b57c273b\n  protects: https://api.acrisure.com/v1/mcp\n- scope: offline_access\n  description: >-\n    Standard OIDC scope. Permits issuance of a refresh token so an agent session can\n    outlive the initial access token.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.acrisure.com/.well-known/oauth-authorization-server\n  standard: true\nsummary:\n  scope_count: 2\n  provider_specific_scopes: 1\n  standard_scopes: 1\n  granularity: coarse\n  granularity_note: >-\n    A single provider-specific scope covers the entire MCP surface. There is no\n    read/write split, no per-resource scope, and no least-privilege gradation, so any\n    agent granted `mcp_user` receives whatever the full tool set can do.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://api.acrisure.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrisure/refs/heads/main/scopes/acrisure-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Insurance
- insurance-brokerage
- Fintech
- employee-benefits
- payroll-hr
- reinsurance
- risk-management
- Cybersecurity
- mortgage
- surety-bonds
- MCP
- Authentication
token_urls:
- https://api.acrisure.com/oauth/token
---
