---
authorization_urls:
- https://auth.share.vendia.com/authorize
description: ''
docs: https://docs.vendia.com/platform/operational/secure-data-sharing/rbac/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Vendia Scopes
name_suffix: OAuth Scopes
note: Vendia's OAuth authorization server advertises only the three standard OIDC scopes. Authorization for data access is NOT carried in OAuth scopes — it is carried in Vendia's own RBAC permission model, which is bound to the credential's assigned role and evaluated per project and workspace. Both layers are recorded here because an agent integrating with the MCP Gateway must satisfy the permission layer, not the scope layer. Only permissions Vendia names explicitly in its public docs are listed.
overview: 'Vendia publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vendia API on a user''s behalf.


  Tokens are issued from https://auth.share.vendia.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vendia
provider_slug: vendia
schemes:
- flows:
  - authorizationUrl: https://auth.share.vendia.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.share.vendia.com/token
  - flow: clientCredentials
    tokenUrl: https://auth.share.vendia.com/token
  issuer: https://auth.share.vendia.com
  name: VendiaOAuth2
  source: well-known/vendia-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC claim set for the authenticated user's profile.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC claim set for the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
slug: vendia-scopes
source_filename: vendia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://auth.share.vendia.com/.well-known/oauth-authorization-server\ndocs: https://docs.vendia.com/platform/operational/secure-data-sharing/rbac/\nnote: >-\n  Vendia's OAuth authorization server advertises only the three standard OIDC scopes.\n  Authorization for data access is NOT carried in OAuth scopes — it is carried in\n  Vendia's own RBAC permission model, which is bound to the credential's assigned role\n  and evaluated per project and workspace. Both layers are recorded here because an\n  agent integrating with the MCP Gateway must satisfy the permission layer, not the\n  scope layer. Only permissions Vendia names explicitly in its public docs are listed.\nschemes:\n- name: VendiaOAuth2\n  source: well-known/vendia-oauth-authorization-server.json\n  issuer: https://auth.share.vendia.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.share.vendia.com/authorize\n    tokenUrl: https://auth.share.vendia.com/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.share.vendia.com/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/vendia-oauth-authorization-server.json]\n- scope: profile\n  description: Standard OIDC claim set for the authenticated user's profile.\n  flows: [authorizationCode]\n  sources: [well-known/vendia-oauth-authorization-server.json]\n- scope: email\n  description: Standard OIDC claim set for the authenticated user's email address.\n  flows: [authorizationCode]\n  sources: [well-known/vendia-oauth-authorization-server.json]\npermissions:\n  model: role-based-access-control\n  bound_to: [project, workspace]\n  docs: https://docs.vendia.com/platform/operational/secure-data-sharing/rbac/\n  named_in_docs:\n  - permission: DATA_READ\n    description: >-\n      Required on a credential for MCP Gateway access to the project and workspace the\n      MCP server is attached\
  \ to.\n    source: https://docs.vendia.com/platform/vendia-mcp-server/authentication/\naccess_policy_actions:\n  model: >-\n    Storage Connections apply a second, Vendia-level access-policy layer on top of AWS\n    IAM. Both layers must allow an operation for it to succeed.\n  docs: https://docs.vendia.com/platform/vendia-mcp-server/storage-connections/access-policies/\n  actions:\n  - action: FILE_READ\n    description: Read/list files matching the policy's glob patterns.\n  - action: FILE_CREATE\n    description: Create new files; explicitly does NOT permit overwriting existing files.\n  - action: FILE_WRITE\n    description: Overwrite existing files; explicitly does NOT permit creating new ones.\n  - action: FILE_DELETE\n    description: Delete files matching the policy's glob patterns.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://auth.share.vendia.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://docs.vendia.com/platform/vendia-mcp-server/storage-connections/mcp-tools/\n\
  \    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendia/refs/heads/main/scopes/vendia-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- MCP
- Model Context Protocol
- Artificial Intelligence
- Data Sharing
- Data Platform
- GraphQL
- Agents
- API Gateway
- Data Governance
token_urls:
- https://auth.share.vendia.com/token
---
