---
api_specs:
- filename: flume-health-console-api-openapi.yml
  format: yaml
  label: Flume Console API
  slug: flume-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-console-api-openapi.yml
authorization_urls:
- https://auth.flumehealth.com/authorize?audience=https://console.flumehealth.com/api
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Flume Health Scopes
name_suffix: OAuth Scopes
note: 'Upgraded from the spec-only derivation. Flume Health publishes NO scopes or permissions reference page — there is nothing to search — so the scope inventory below is assembled from three machine-readable sources: the securityDefinitions block of the published contract (3 scopes), the live authorization-server metadata (14 scopes), and the MCP protected-resource metadata (4 scopes). The important finding is that all of them are standard OIDC identity scopes. Flume declares NO resource or permission scopes of its own — no read/write scope, no per-resource scope, nothing that constrains what a bearer token may do to accounts, endpoints, source files, or the Context knowledge graph. Authorization is not expressed in the token''s scope; it is enforced server-side through the X-Flume-Account-ID account scoping and the Context Discovery approval/session model. An agent cannot request least privilege from this API, because least privilege is not expressible in its scopes.'
overview: 'Flume Health publishes 14 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flume Health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flume Health
provider_slug: flume-health
schemes:
- flows:
  - authorizationUrl: https://auth.flumehealth.com/authorize?audience=https://console.flumehealth.com/api
    flow: implicit
  name: OAuth2Implicit
  source: openapi/flume-health-console-api-openapi.yml
- issuer: https://auth.flumehealth.com/
  name: Flume authorization server
  source: well-known/flume-health-oauth-authorization-server.json
- name: MCP protected resource
  resource: https://console.flumehealth.com/api/v1/context/mcp
  source: well-known/flume-health-oauth-protected-resource.json
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OpenID Connect scope. Requests an ID token.
  flows:
  - implicit
  - authorization_code
  scope: openid
- description: User profile information.
  flows:
  - implicit
  - authorization_code
  scope: profile
- description: User email address.
  flows:
  - implicit
  - authorization_code
  scope: email
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorization_code
  - device_code
  scope: offline_access
- description: Standard OIDC claim scope.
  flows: []
  scope: name
- description: Standard OIDC claim scope.
  flows: []
  scope: given_name
- description: Standard OIDC claim scope.
  flows: []
  scope: family_name
- description: Standard OIDC claim scope.
  flows: []
  scope: nickname
- description: Standard OIDC claim scope.
  flows: []
  scope: email_verified
- description: Standard OIDC claim scope.
  flows: []
  scope: picture
- description: Standard OIDC claim scope.
  flows: []
  scope: created_at
- description: Standard OIDC claim scope (linked identity providers).
  flows: []
  scope: identities
- description: Standard OIDC claim scope.
  flows: []
  scope: phone
- description: Standard OIDC claim scope.
  flows: []
  scope: address
slug: flume-health-scopes
source_filename: flume-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: >-\n  https://auth.flumehealth.com/.well-known/oauth-authorization-server +\n  https://console.flumehealth.com/.well-known/oauth-protected-resource + openapi/flume-health-console-api-openapi.yml\nnote: >-\n  Upgraded from the spec-only derivation. Flume Health publishes NO scopes or permissions reference page — there is\n  nothing to search — so the scope inventory below is assembled from three machine-readable sources: the\n  securityDefinitions block of the published contract (3 scopes), the live authorization-server metadata (14\n  scopes), and the MCP protected-resource metadata (4 scopes). The important finding is that all of them are\n  standard OIDC identity scopes. Flume declares NO resource or permission scopes of its own — no read/write scope,\n  no per-resource scope, nothing that constrains what a bearer token may do to accounts, endpoints, source files, or\n  the Context knowledge graph. Authorization is not expressed\
  \ in the token's scope; it is enforced server-side\n  through the X-Flume-Account-ID account scoping and the Context Discovery approval/session model. An agent cannot\n  request least privilege from this API, because least privilege is not expressible in its scopes.\ndocs: null\nscope_model: identity-only\nresource_scopes_declared: 0\n\nschemes:\n- name: OAuth2Implicit\n  source: openapi/flume-health-console-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.flumehealth.com/authorize?audience=https://console.flumehealth.com/api\n- name: Flume authorization server\n  source: well-known/flume-health-oauth-authorization-server.json\n  issuer: https://auth.flumehealth.com/\n- name: MCP protected resource\n  source: well-known/flume-health-oauth-protected-resource.json\n  resource: https://console.flumehealth.com/api/v1/context/mcp\n\nscopes:\n- scope: openid\n  description: OpenID Connect scope. Requests an ID token.\n  kind: identity\n  flows: [implicit, authorization_code]\n\
  \  surfaces: [rest, mcp]\n  sources:\n  - openapi/flume-health-console-api-openapi.yml\n  - well-known/flume-health-oauth-authorization-server.json\n  - well-known/flume-health-oauth-protected-resource.json\n- scope: profile\n  description: User profile information.\n  kind: identity\n  flows: [implicit, authorization_code]\n  surfaces: [rest, mcp]\n  sources:\n  - openapi/flume-health-console-api-openapi.yml\n  - well-known/flume-health-oauth-authorization-server.json\n  - well-known/flume-health-oauth-protected-resource.json\n- scope: email\n  description: User email address.\n  kind: identity\n  flows: [implicit, authorization_code]\n  surfaces: [rest, mcp]\n  sources:\n  - openapi/flume-health-console-api-openapi.yml\n  - well-known/flume-health-oauth-authorization-server.json\n  - well-known/flume-health-oauth-protected-resource.json\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without user interaction.\n  kind: identity\n\
  \  flows: [authorization_code, device_code]\n  surfaces: [mcp]\n  note: Advertised by the authorization server and by the MCP protected-resource metadata, but NOT declared in the OpenAPI securityDefinitions.\n  sources:\n  - well-known/flume-health-oauth-authorization-server.json\n  - well-known/flume-health-oauth-protected-resource.json\n- scope: name\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: given_name\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: family_name\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: nickname\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: email_verified\n  description: Standard OIDC claim\
  \ scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: picture\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: created_at\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: identities\n  description: Standard OIDC claim scope (linked identity providers).\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: phone\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n- scope: address\n  description: Standard OIDC claim scope.\n  kind: identity\n  sources: [well-known/flume-health-oauth-authorization-server.json]\n\nauthorization_beyond_scopes:\n- mechanism: account scoping\n  detail: The X-Flume-Account-ID request header selects the health-plan\
  \ account; 122 of 153 operations require it. Wrong or unpermitted account yields 403.\n- mechanism: Context Discovery sessions\n  detail: >-\n    Access to a customer's data estate for tooling is granted as a time-boxed, approver-gated session\n    (23 operations under /api/v1/context/discovery/). Grant types include subscription_access for AI CLI tools.\n    Sessions can be approved, denied, extended, cancelled and revoked, and launches are written to an audit log.\n    This — not OAuth scope — is where Flume expresses fine-grained agent authorization.\n- mechanism: query-engine grants\n  detail: /api/v1/users/{id}/query-engine-grant and /query-engine-revoke gate a user's access to the query engine.\n\nevidence:\n- url: https://auth.flumehealth.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://console.flumehealth.com/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://console.flumehealth.com/api/docs/docs.json\n  http_status: 200\nchecked:\
  \ '2026-08-16'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/scopes/flume-health-scopes.yml
summary_line: 14 scopes · implicit
tags:
- Healthcare
- Health Plans
- Payers
- Healthcare Data
- Data Integration
- iPaaS
- Eligibility
- Claims
- Knowledge Graph
- MCP
- agent-native
- Authentication
- Data Engineering
- Interoperability
token_urls: []
---
