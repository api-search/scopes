---
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-environments-api-openapi.yml
  format: yaml
  label: flagsmith Environments API
  slug: flagsmith-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-environments-api-openapi.yml
- filename: flagsmith-features-api-openapi.yml
  format: yaml
  label: flagsmith Features API
  slug: flagsmith-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-features-api-openapi.yml
- filename: flagsmith-identities-api-openapi.yml
  format: yaml
  label: flagsmith Identities API
  slug: flagsmith-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-identities-api-openapi.yml
- filename: flagsmith-organisations-api-openapi.yml
  format: yaml
  label: flagsmith Organisations API
  slug: flagsmith-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-organisations-api-openapi.yml
- filename: flagsmith-projects-api-openapi.yml
  format: yaml
  label: flagsmith Projects API
  slug: flagsmith-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-projects-api-openapi.yml
- filename: flagsmith-segments-api-openapi.yml
  format: yaml
  label: flagsmith Segments API
  slug: flagsmith-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-segments-api-openapi.yml
- filename: flagsmith-users-api-openapi.yml
  format: yaml
  label: flagsmith Users API
  slug: flagsmith-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-users-api-openapi.yml
- filename: flagsmith-webhooks-api-openapi.yml
  format: yaml
  label: flagsmith Webhooks API
  slug: flagsmith-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.flagsmith.com/integrating-with-flagsmith/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Flagsmith Scopes
name_suffix: OAuth Scopes
note: 'Read from the provider''s own RFC 8414 metadata rather than derived — derive-oauth-scopes.py finds nothing because the OpenAPI declares its security schemes as apiKey/http and never as oauth2, so the OAuth surface is invisible from the contract alone. It is only discoverable from the .well-known documents, which is exactly why they were probed. Two scopes, coarse-grained: there is no per-resource or read/write split, so an agent granted `mcp` can reach every tool the deployment exposes, and one granted `admin-api` can reach the Management API within the granting user''s own permissions. Fine-grained restriction is done with Flagsmith''s RBAC roles and permission groups, not with OAuth scopes.'
overview: 'Flagsmith uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flagsmith
provider_slug: flagsmith
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: flagsmith-scopes
source_filename: flagsmith-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://api.flagsmith.com/.well-known/oauth-authorization-server (HTTP 200, fetched 2026-09-17)\ndocs: https://docs.flagsmith.com/integrating-with-flagsmith/mcp-server\nauthorization_server: https://api.flagsmith.com\nissuer: https://api.flagsmith.com\nendpoints:\n  authorization: https://app.flagsmith.com/oauth/authorize/\n  token: https://api.flagsmith.com/o/token/\n  registration: https://api.flagsmith.com/o/register/\n  revocation: https://api.flagsmith.com/o/revoke_token/\n  introspection: https://api.flagsmith.com/o/introspect/\ngrant_types: [authorization_code, refresh_token]\nresponse_types: [code]\npkce: [S256]\ntoken_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\nscope_count: 2\nnote: >-\n  Read from the provider's own RFC 8414 metadata rather than derived — derive-oauth-scopes.py finds\n  nothing because the OpenAPI declares its security schemes as apiKey/http and never as oauth2, so\n  the\
  \ OAuth surface is invisible from the contract alone. It is only discoverable from the\n  .well-known documents, which is exactly why they were probed. Two scopes, coarse-grained: there is\n  no per-resource or read/write split, so an agent granted `mcp` can reach every tool the deployment\n  exposes, and one granted `admin-api` can reach the Management API within the granting user's own\n  permissions. Fine-grained restriction is done with Flagsmith's RBAC roles and permission groups,\n  not with OAuth scopes.\nscopes:\n- name: mcp\n  description: >-\n    Access to the Flagsmith MCP server at https://mcp.flagsmith.com. This is the scope an MCP client\n    requests during the interactive OAuth flow. Confirmed independently by the RFC 9728\n    protected-resource document on the MCP host, whose scopes_supported is [mcp].\n  surface: https://mcp.flagsmith.com\n  granularity: coarse\n  evidence: https://mcp.flagsmith.com/.well-known/oauth-protected-resource\n- name: admin-api\n  description:\
  \ >-\n    Access to the Flagsmith Management API at https://api.flagsmith.com/api/v1. Requests act with the\n    permissions of the authorising user — the provider states administrator privileges are not\n    required and that any organisation member can use the Management API within the scope of their\n    own permissions.\n  surface: https://api.flagsmith.com/api/v1\n  granularity: coarse\n  evidence: https://docs.flagsmith.com/integrating-with-flagsmith/flagsmith-api-overview/management-api/\neffective_authorization:\n  model: RBAC\n  note: >-\n    The real authorization boundary is Flagsmith's own role/permission system (Permissions tag, 34\n    operations; custom roles and permission groups on Enterprise), layered under whichever OAuth\n    scope or API key was presented. An OAuth token never widens what its user could already do.\n  see: authentication/flagsmith-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/scopes/flagsmith-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Feature Flags
- Remote Config
- Release Management
- A/B Testing
- Experimentation
- Segmentation
- Developer Tools
- DevOps
- Open-Source
- Software-as-a-Service
- MCP
- Agent Ready
token_urls: []
---
