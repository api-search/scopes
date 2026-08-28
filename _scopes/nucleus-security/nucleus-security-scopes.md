---
api_specs:
- filename: nucleus-security-vulnerability-intelligence-openapi.yml
  format: yaml
  label: Nucleus Security Vulnerability Intelligence API
  slug: nucleus-security-vulnerability-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nucleus-security/refs/heads/main/openapi/nucleus-security-vulnerability-intelligence-openapi.yml
authorization_urls: []
description: The only OAuth scope Nucleus Security publishes machine-readably is the single `mcp` scope advertised by the RFC 8414 authorization-server metadata on nucleussec.com. The platform's real authorization model is not scope-based - it is RBAC plus Asset Group Access Control, evaluated server-side per project.
docs: https://help.nucleussec.com/docs/users-roles-and-permissions
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Nucleus Security Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nucleus Security publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nucleus Security API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nucleus Security
provider_slug: nucleus-security
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an MCP client access to the protected resource https://nucleussec.com/wp-json/mcp/mcp-oauth-server. The single scope published by the authorization server; it is not further decomposed into read/write or per-resource scopes.
  flows: []
  scope: mcp
slug: nucleus-security-scopes
source_filename: nucleus-security-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Nucleus Security OAuth Scopes\ndescription: >-\n  The only OAuth scope Nucleus Security publishes machine-readably is the single `mcp`\n  scope advertised by the RFC 8414 authorization-server metadata on nucleussec.com. The\n  platform's real authorization model is not scope-based - it is RBAC plus Asset Group\n  Access Control, evaluated server-side per project.\ngenerated: '2026-08-26'\nmethod: probed\nsource: https://nucleussec.com/.well-known/oauth-authorization-server\ndocs: https://help.nucleussec.com/docs/users-roles-and-permissions\nx-evidence:\n  url: https://nucleussec.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-26'\nauthorization_server:\n  issuer: https://nucleussec.com\n  authorization_endpoint: https://nucleussec.com/oauth/authorize\n  token_endpoint: https://nucleussec.com/oauth/token\n  revocation_endpoint: https://nucleussec.com/oauth/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported:\
  \ [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\nscopes:\n- scope: mcp\n  description: >-\n    Grants an MCP client access to the protected resource\n    https://nucleussec.com/wp-json/mcp/mcp-oauth-server. The single scope published by the\n    authorization server; it is not further decomposed into read/write or per-resource scopes.\n  resource: https://nucleussec.com/wp-json/mcp/mcp-oauth-server\n  source: RFC 8414 scopes_supported\nscope_count: 1\nauthorization_model:\n  primary: rbac\n  note: >-\n    Nucleus does not express platform API authorization as OAuth scopes. Access is granted\n    through roles assigned per project (RBAC) and narrowed by Asset Group Access Control\n    (AGAC). API keys and MCP sessions both inherit the owning principal's role, and\n    permissions are re-evaluated at query time, so an administrator changing\
  \ a role changes\n    what an already-issued key or session can reach.\n  dedicated_permissions:\n  - name: API Access\n    effect: >-\n      Required for a user or role to hold an API key at all. Disabling it also disables MCP\n      for that principal.\n  - name: MCP access\n    effect: >-\n      Dedicated permission in the Nucleus role model governing MCP Server use. Enabled by\n      default on all out-of-the-box roles.\n  - name: Organization Admin\n    effect: Required to create API-only service accounts and view their keys.\n  docs: https://help.nucleussec.com/docs/users-roles-and-permissions\ngaps:\n- >-\n  No scopes reference page exists for the platform API because the platform API is not\n  scope-based. The permissions reference is the roles documentation cited above.\n- >-\n  The product MCP server at https://[instance].nucleussec.com/nucleus/mcp is per-tenant;\n  its authorization-server metadata was not probed because no shared instance host exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nucleus-security/refs/heads/main/scopes/nucleus-security-scopes.yml
summary_line: 1 scope
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Exposure Management
- Risk Management
- Threat Intelligence
- Compliance
- DevSecOps
- MCP
token_urls: []
---
