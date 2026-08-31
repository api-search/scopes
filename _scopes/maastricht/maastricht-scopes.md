---
api_specs:
- filename: maastricht-oai-pmh-openapi.yml
  format: yaml
  label: Maastricht University Research Portal OAI-PMH
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/openapi/maastricht-oai-pmh-openapi.yml
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the Maastricht University ADFS identity provider. Read verbatim from the institution's own public discovery document on 2026-08-30 — not inferred and not a vendor's default list. These govern access to UM-affiliated relying parties; they are NOT scopes on a public data API, and Maastricht publishes no scoped public data API.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Maastricht Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Maastricht University publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Maastricht University API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Maastricht University
provider_slug: maastricht
schemes: []
scope_count: 10
scope_names:
- openid
- profile
- email
- allatclaims
- aza
- ugs
- user_impersonation
- logon_cert
- vpn_cert
- winhello_cert
scopes:
- description: Standard OpenID Connect scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: ADFS scope returning all configured claims for the relying party.
  flows: []
  scope: allatclaims
- description: ADFS broker-client scope used for primary refresh-token flows.
  flows: []
  scope: aza
- description: ADFS scope used by the Microsoft Universal Group Service.
  flows: []
  scope: ugs
- description: Delegated access on behalf of the signed-in user.
  flows: []
  scope: user_impersonation
- description: Issues a logon certificate for the authenticated user.
  flows: []
  scope: logon_cert
- description: Issues a VPN certificate for the authenticated user.
  flows: []
  scope: vpn_cert
- description: Issues a Windows Hello for Business certificate.
  flows: []
  scope: winhello_cert
slug: maastricht-scopes
source_filename: maastricht-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "provider: Maastricht University\nproviderId: maastricht\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://login.maastrichtuniversity.nl/adfs/.well-known/openid-configuration\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the Maastricht University ADFS identity provider.\n  Read verbatim from the institution's own public discovery document on 2026-08-30 — not inferred\n  and not a vendor's default list. These govern access to UM-affiliated relying parties; they are\n  NOT scopes on a public data API, and Maastricht publishes no scoped public data API.\napi: Maastricht University ADFS (OpenID Connect)\nbaseURL: https://login.maastrichtuniversity.nl/adfs\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n- scope: profile\n  description: Standard OIDC profile claims.\n- scope: email\n  description: Standard OIDC email claim.\n- scope: allatclaims\n  description: ADFS scope returning all configured claims\
  \ for the relying party.\n- scope: aza\n  description: ADFS broker-client scope used for primary refresh-token flows.\n- scope: ugs\n  description: ADFS scope used by the Microsoft Universal Group Service.\n- scope: user_impersonation\n  description: Delegated access on behalf of the signed-in user.\n- scope: logon_cert\n  description: Issues a logon certificate for the authenticated user.\n- scope: vpn_cert\n  description: Issues a VPN certificate for the authenticated user.\n- scope: winhello_cert\n  description: Issues a Windows Hello for Business certificate.\nclaims:\n- aud\n- iss\n- iat\n- exp\n- auth_time\n- nonce\n- at_hash\n- c_hash\n- sub\n- upn\n- unique_name\n- pwd_url\n- pwd_exp\n- mfa_auth_time\n- sid\n- nbf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/scopes/maastricht-scopes.yml
summary_line: 10 scopes
tags:
- University
- Higher Education
- Education
- Netherlands
- Europe
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Open Access
- Public Research University
token_urls: []
---
