---
api_specs:
- filename: corestack-external-api-openapi-original.json
  format: json
  label: CoreStack External API
  slug: corestack-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/openapi/corestack-external-api-openapi-original.json
authorization_urls:
- https://cloud.corestack.io/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Corestack Scopes
name_suffix: OAuth Scopes
note: 'CoreStack''s 838-operation REST contract declares NO oauth2 security scheme — it is key-and-token only, and authorization is role-based rather than scope-based, so there is no REST scope surface to derive. The only OAuth surface on the estate is the one the unified MCP server stood up, and it advertises exactly three OIDC-standard scopes. Those scopes carry identity, not capability: what a caller may actually do is decided entirely by their CoreStack RBAC role, not by the token''s scope.'
overview: 'CoreStack uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://cloud.corestack.io/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreStack
provider_slug: corestack
schemes:
- bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://cloud.corestack.io/mcp/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    pkce: S256
    response_types:
    - code
    tokenUrl: https://cloud.corestack.io/mcp/oauth/token
  issuer: https://cloud.corestack.io/mcp
  name: mcp_oauth
  protected_resource: https://cloud.corestack.io/mcp
  registration_endpoint: https://cloud.corestack.io/mcp/oauth/register
  source: well-known/corestack-oauth-authorization-server.json
  surface: mcp
scope_count: 0
scope_names: []
scopes: []
slug: corestack-scopes
source_filename: corestack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://cloud.corestack.io/.well-known/oauth-authorization-server\nnote: >-\n  CoreStack's 838-operation REST contract declares NO oauth2 security scheme — it is key-and-token\n  only, and authorization is role-based rather than scope-based, so there is no REST scope surface to\n  derive. The only OAuth surface on the estate is the one the unified MCP server stood up, and it\n  advertises exactly three OIDC-standard scopes. Those scopes carry identity, not capability: what a\n  caller may actually do is decided entirely by their CoreStack RBAC role, not by the token's scope.\n\nschemes:\n- name: mcp_oauth\n  surface: mcp\n  source: well-known/corestack-oauth-authorization-server.json\n  issuer: https://cloud.corestack.io/mcp\n  protected_resource: https://cloud.corestack.io/mcp\n  bearer_methods_supported:\n  - header\n  dynamic_client_registration: true\n  registration_endpoint: https://cloud.corestack.io/mcp/oauth/register\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.corestack.io/mcp/oauth/authorize\n    tokenUrl: https://cloud.corestack.io/mcp/oauth/token\n    pkce: S256\n    response_types:\n    - code\n    grant_types:\n    - authorization_code\n\nscopes:\n- name: openid\n  description: OIDC authentication — issues an ID token identifying the CoreStack user.\n  spec: OpenID Connect Core 1.0\n- name: email\n  description: Releases the authenticated user's email address claim.\n  spec: OpenID Connect Core 1.0\n- name: profile\n  description: Releases the authenticated user's basic profile claims.\n  spec: OpenID Connect Core 1.0\n\nscope_count: 3\n\nauthorization_note: >-\n  There is no per-tool, per-domain or per-operation scope. An agent authorized against this server\n  can reach every one of the 100 MCP tools its user's role permits, including the four tools the\n  provider marks Destructive (submit_assessment_answer, create_workload, send_agent_query, file_bug).\n  Consent\
  \ at the token layer is therefore all-or-nothing: the user cannot grant read-only FinOps\n  access to an agent without also granting whatever else their role allows. Narrowing this would mean\n  either scoping the OAuth server by domain or issuing a reduced-privilege service account.\n\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://cloud.corestack.io/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestack/refs/heads/main/scopes/corestack-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cloud Governance
- FinOps
- Cloud Cost Management
- Cloud Security Posture Management
- Compliance
- Multi-Cloud
- CNAPP
- Policy as Code
- cloudops
- MCP
- agent-native
- Kubernetes
token_urls:
- https://cloud.corestack.io/mcp/oauth/token
---
