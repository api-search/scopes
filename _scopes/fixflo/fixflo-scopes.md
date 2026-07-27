---
api_specs:
- filename: fixflo-api-v2-openapi.yml
  format: yaml
  label: Fixflo API v2
  slug: fixflo-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixflo/refs/heads/main/openapi/fixflo-api-v2-openapi.yml
authorization_urls: []
description: ''
docs: https://api.fixflo.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fixflo Scopes
name_suffix: OAuth Scopes
note: The documented Fixflo v2 REST API has NO scope surface — it is authorised by a single opaque bearer token whose privileges are those of the Fixflo user who generated it, and the published OpenAPI declares no oauth2 security scheme. The scopes below are the real, anonymously published scopes of the SEPARATE Fixflo application authorization server at api.fixflo.com (RFC 8414 metadata + OIDC discovery). They govern the Fixflo web application login, not v2 REST authorisation. Recorded because they are genuinely published; not presented as API scopes.
overview: 'Fixflo publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fixflo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fixflo
provider_slug: fixflo
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Request an ID token and the OpenID Connect authentication response.
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims about the authenticated Fixflo user (name, given_name, family_name, preferred_username).
  flows:
  - authorizationCode
  scope: profile
- description: The authenticated Fixflo user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorizationCode
  scope: offline_access
slug: fixflo-scopes
source_filename: fixflo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: well-known/fixflo-oauth-authorization-server.json\ndocs: https://api.fixflo.com/.well-known/openid-configuration\nscope: application-login-only\nnote: >-\n  The documented Fixflo v2 REST API has NO scope surface — it is authorised by a\n  single opaque bearer token whose privileges are those of the Fixflo user who\n  generated it, and the published OpenAPI declares no oauth2 security scheme.\n  The scopes below are the real, anonymously published scopes of the SEPARATE\n  Fixflo application authorization server at api.fixflo.com (RFC 8414 metadata +\n  OIDC discovery). They govern the Fixflo web application login, not v2 REST\n  authorisation. Recorded because they are genuinely published; not presented as\n  API scopes.\nauthorization_server:\n  issuer: https://api.fixflo.com/\n  metadata:\n  - https://api.fixflo.com/.well-known/oauth-authorization-server\n  - https://api.fixflo.com/.well-known/openid-configuration\n  authorizationUrl:\
  \ https://api.fixflo.com/api/oauth2/authorize\n  tokenUrl: https://api.fixflo.com/api/oauth2/token\n  introspectionUrl: https://api.fixflo.com/api/oauth2/introspection\n  grant_types:\n  - authorization_code\n  - password\n  - refresh_token\n  pkce:\n  - S256\n  - plain\nscopes:\n- scope: openid\n  description: Request an ID token and the OpenID Connect authentication response.\n  flows: [authorizationCode]\n  sources: [well-known/fixflo-oauth-authorization-server.json]\n- scope: profile\n  description: >-\n    Profile claims about the authenticated Fixflo user (name, given_name,\n    family_name, preferred_username).\n  flows: [authorizationCode]\n  sources: [well-known/fixflo-oauth-authorization-server.json]\n- scope: email\n  description: The authenticated Fixflo user's email claim.\n  flows: [authorizationCode]\n  sources: [well-known/fixflo-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without\
  \ user interaction.\n  flows: [authorizationCode]\n  sources: [well-known/fixflo-oauth-authorization-server.json]\nrest_api_scopes:\n  count: 0\n  reason: >-\n    Fixflo API v2 uses a single-privilege bearer token, not scoped OAuth. There\n    is no documented per-resource or per-verb scope, and no way to request a\n    reduced-privilege API token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixflo/refs/heads/main/scopes/fixflo-scopes.yml
summary_line: 4 scopes
tags:
- Real Estate
- United Kingdom
- Property Management
- PropTech
- Repairs and Maintenance
- Block Management
- Lettings
- Rentals
- Commercial Real Estate
- Contractors
token_urls: []
---
