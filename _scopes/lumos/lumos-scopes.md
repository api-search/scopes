---
api_specs:
- filename: lumos-openapi.json
  format: json
  label: Lumos REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-openapi.json
- filename: lumos-accesspolicies-api-openapi.yml
  format: yaml
  label: Lumos AccessPolicies API
  slug: lumos-accesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accesspolicies-api-openapi.yml
- filename: lumos-accessrequests-api-openapi.yml
  format: yaml
  label: Lumos AccessRequests API
  slug: lumos-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessrequests-api-openapi.yml
- filename: lumos-accessreviews-api-openapi.yml
  format: yaml
  label: Lumos AccessReviews API
  slug: lumos-accessreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessreviews-api-openapi.yml
- filename: lumos-accounts-api-openapi.yml
  format: yaml
  label: Lumos Accounts API
  slug: lumos-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accounts-api-openapi.yml
- filename: lumos-activity-api-openapi.yml
  format: yaml
  label: Lumos Activity API
  slug: lumos-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-activity-api-openapi.yml
- filename: lumos-apps-api-openapi.yml
  format: yaml
  label: Lumos Apps API
  slug: lumos-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-apps-api-openapi.yml
- filename: lumos-appstore-api-openapi.yml
  format: yaml
  label: Lumos AppStore API
  slug: lumos-appstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-appstore-api-openapi.yml
- filename: lumos-groups-api-openapi.yml
  format: yaml
  label: Lumos Groups API
  slug: lumos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-groups-api-openapi.yml
- filename: lumos-preapprovalrules-api-openapi.yml
  format: yaml
  label: Lumos PreApprovalRules API
  slug: lumos-preapprovalrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-preapprovalrules-api-openapi.yml
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-users-api-openapi.yml
  format: yaml
  label: Lumos Users API
  slug: lumos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-users-api-openapi.yml
- filename: lumos-utility-api-openapi.yml
  format: yaml
  label: Lumos Utility API
  slug: lumos-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-utility-api-openapi.yml
- filename: lumos-vendors-api-openapi.yml
  format: yaml
  label: Lumos Vendors API
  slug: lumos-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendors-api-openapi.yml
- filename: lumos-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Webhooks API
  slug: lumos-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-webhooks-api-openapi.yml
authorization_urls: []
description: Lumos publishes its OAuth scope vocabulary in RFC 8414 authorization-server metadata rather than in the OpenAPI, which declares only HTTPBearer. These 14 scopes govern the two hosted MCP servers; the REST API itself is authenticated with an lsk_ API key and is NOT scope-partitioned.
docs: https://developers.lumos.com/docs/lumos-admin-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Lumos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lumos uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lumos
provider_slug: lumos
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: lumos-scopes
source_filename: lumos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://api.lumos.com/.well-known/oauth-authorization-server (302 -> b.app.lumosidentity.com),\n  https://api.lumos.com/.well-known/oauth-protected-resource/mcp/user,\n  https://api.lumos.com/.well-known/oauth-protected-resource/mcp/admin\ndocs: https://developers.lumos.com/docs/lumos-admin-mcp\ndescription: >-\n  Lumos publishes its OAuth scope vocabulary in RFC 8414 authorization-server metadata rather than in\n  the OpenAPI, which declares only HTTPBearer. These 14 scopes govern the two hosted MCP servers; the\n  REST API itself is authenticated with an lsk_ API key and is NOT scope-partitioned.\nissuer: https://b.app.lumosidentity.com\nflows:\n  authorization_code:\n    authorizationUrl: https://b.app.lumosidentity.com/b/oauth/authorize\n    tokenUrl: https://b.app.lumosidentity.com/b/oauth/token\n    revocationUrl: https://b.app.lumosidentity.com/b/oauth/revoke\n    registrationUrl: https://b.app.lumosidentity.com/b/oauth/register\n\
  \    pkce: S256\n    refresh_token: true\nscope_count: 14\nscopes:\n- name: lumos:user:read\n  description: Read the signing-in user's own apps, requestable permissions, and access requests.\n  resource: https://api.lumos.com/mcp/user\n- name: lumos:user:write\n  description: Submit and cancel access requests on the signing-in user's behalf.\n  resource: https://api.lumos.com/mcp/user\n- name: lumos:admin:access-policies:read\n  description: Read domain access policies.\n  resource: https://api.lumos.com/mcp/admin\n- name: lumos:admin:access-policies:write\n  description: Create, update, and delete domain access policies.\n  resource: https://api.lumos.com/mcp/admin\n- name: lumos:admin:appstore:read\n  description: Inspect AppStore apps, requestable permissions, and approval configuration.\n  resource: https://api.lumos.com/mcp/admin\n  toolset: appstore\n- name: lumos:admin:appstore:write\n  description: Configure AppStore approval workflows and permission configuration.\n  resource:\
  \ https://api.lumos.com/mcp/admin\n  toolset: appstore\n- name: lumos:admin:knowledge-hub:read\n  description: List and read Knowledge Hub entries for the domain.\n  resource: https://api.lumos.com/mcp/admin\n  toolset: knowledge-hub\n- name: lumos:admin:knowledge-hub:write\n  description: Create, update, and archive Knowledge Hub entries.\n  resource: https://api.lumos.com/mcp/admin\n  toolset: knowledge-hub\n- name: lumos:admin:mcp-governance:read\n  description: Read Lumos MCP governance configuration.\n  resource: https://api.lumos.com/mcp/admin\n  note: >-\n    Advertised by the authorization server but no matching toolset is documented on the admin MCP\n    page. Recorded as published, not as reachable.\n- name: lumos:admin:mcp-governance:write\n  description: Write Lumos MCP governance configuration.\n  resource: https://api.lumos.com/mcp/admin\n  note: Advertised by the authorization server; no documented toolset yet.\n- name: lumos:admin:task-center:read\n  description: Read manual\
  \ approval, provisioning, and error tasks.\n  resource: https://api.lumos.com/mcp/admin\n  toolset: task-center\n- name: lumos:admin:task-center:write\n  description: Act on, reassign, complete, and dismiss tasks.\n  resource: https://api.lumos.com/mcp/admin\n  toolset: task-center\n- name: lumos:admin:workflows:read\n  description: Read workflow configuration.\n  resource: https://api.lumos.com/mcp/admin\n- name: lumos:admin:workflows:write\n  description: Write workflow configuration.\n  resource: https://api.lumos.com/mcp/admin\nx-evidence:\n- url: https://api.lumos.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://api.lumos.com/.well-known/oauth-protected-resource/mcp/user\n  status: 200\n- url: https://api.lumos.com/.well-known/oauth-protected-resource/mcp/admin\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/scopes/lumos-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
token_urls: []
---
