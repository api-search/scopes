---
api_specs:
- filename: pavoot-api-openapi.json
  format: json
  label: Pavoot Application API
  slug: pavoot-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/openapi/pavoot-api-openapi.json
authorization_urls: []
description: ''
docs: https://clerk.com/docs/oauth/scoped-access
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pavoot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pavoot uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pavoot
provider_slug: pavoot
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: pavoot-scopes
source_filename: pavoot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.pavoot.com/.well-known/openid-configuration\ndocs: https://clerk.com/docs/oauth/scoped-access\nname: Pavoot OAuth 2.0 / OIDC scopes\nsummary: >-\n  Scopes read verbatim from Pavoot's own OAuth authorization-server metadata at\n  clerk.pavoot.com. These are the identity scopes of the Clerk instance that\n  issues Pavoot sessions — they are NOT permissions over the api.pavoot.com\n  application surface, which uses a database-backed RBAC model instead.\nauthorization_server:\n  issuer: https://clerk.pavoot.com\n  authorization_endpoint: https://clerk.pavoot.com/oauth/authorize\n  token_endpoint: https://clerk.pavoot.com/oauth/token\n  introspection_endpoint: https://clerk.pavoot.com/oauth/token_info\n  revocation_endpoint: https://clerk.pavoot.com/oauth/token/revoke\n  userinfo_endpoint: https://clerk.pavoot.com/oauth/userinfo\n  jwks_uri: https://clerk.pavoot.com/.well-known/jwks.json\n  grant_types_supported:\n \
  \ - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  service_documentation: https://clerk.com/docs/oauth/scoped-access\nscope_count: 7\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token identifying the end user.\n  standard: OIDC Core 1.0\n- name: profile\n  description: Basic profile claims (name, given_name, family_name,\n    preferred_username, picture).\n  standard: OIDC Core 1.0\n- name: email\n  description: Email address and email_verified claim.\n  standard: OIDC Core 1.0\n- name: offline_access\n  description: Issue a refresh token so the client can act after the user leaves.\n  standard: OIDC Core 1.0\n- name: public_metadata\n  description: Read the Clerk user's public metadata.\n  standard: Clerk-specific\n- name: private_metadata\n  description: Read the Clerk user's private metadata.\n  standard: Clerk-specific\n- name:\
  \ 'user:org:read'\n  description: Read the user's organization membership.\n  standard: Clerk-specific\nclaims_supported:\n- sub\n- aud\n- iss\n- exp\n- iat\n- email\n- email_verified\n- given_name\n- family_name\n- name\n- preferred_username\n- picture\n- org_id\napi_authorization_note: >-\n  The api.pavoot.com OpenAPI declares no securitySchemes and no per-operation\n  security, and none of the seven scopes above appear anywhere in the spec. API\n  authorization is enforced by Pavoot's own permission system — role and user\n  permission matrices (/org/permissions/role-matrix, /org/permissions/user-matrix),\n  per-task permissions (/org/permissions/tasks), permission presets with a\n  settable org default, an effective-permissions read (/getEffectivePermissions,\n  /getEffectiveOrgPermissions) and a middleware gate (/checkRouteAccess). Those\n  permission names are not published anywhere anonymous, so they cannot be\n  enumerated without an authenticated session.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/scopes/pavoot-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Events
- Event Management
- Marketing
- AI Agent
- Attendee Intelligence
- GTM
- Field Marketing
- Pipeline
token_urls: []
---
