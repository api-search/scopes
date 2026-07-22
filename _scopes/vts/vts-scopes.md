---
api_specs:
- filename: vts-openapi.yml
  format: yaml
  label: VTS Lease API
  slug: vts-lease-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/openapi/vts-openapi.yml
authorization_urls:
- https://sandbox.vts.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Vts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VTS publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the VTS API on a user''s behalf.


  Tokens are issued from https://sandbox.vts.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VTS
provider_slug: vts
schemes:
- description: OAuth 2.0 Authorization Code flow with PKCE (VTS Activate / OIDC).
  flows:
  - authorizationUrl: https://sandbox.vts.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.vts.com/oauth/token
  name: oauth2
  source: openapi/vts-openapi.yml
scope_count: 4
scope_names:
- email
- openid
- profile
- read_write
scopes:
- description: Email claim
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Read and write access
  flows:
  - authorizationCode
  scope: read_write
slug: vts-scopes
source_filename: vts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vts-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/vts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.vts.com/oauth/authorize\n    tokenUrl: https://sandbox.vts.com/oauth/token\n  description: OAuth 2.0 Authorization Code flow with PKCE (VTS Activate / OIDC).\nscopes:\n- scope: email\n  description: Email claim\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vts-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vts-openapi.yml\n- scope: profile\n  description: Profile claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vts-openapi.yml\n- scope: read_write\n  description: Read and write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vts/refs/heads/main/scopes/vts-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commercial Real Estate
- PropTech
- Real Estate
- Leasing
- Asset Management
- Property Management
- Tenant Experience
token_urls:
- https://sandbox.vts.com/oauth/token
---
