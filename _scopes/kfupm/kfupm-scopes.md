---
api_specs:
- filename: kfupm-discovery-api-openapi.yml
  format: yaml
  label: King Fahd University of Petroleum & Minerals Discovery API
  slug: kfupm-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-discovery-api-openapi.yml
- filename: kfupm-export-api-openapi.yml
  format: yaml
  label: King Fahd University of Petroleum & Minerals Export API
  slug: kfupm-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-export-api-openapi.yml
- filename: kfupm-oai-pmh-api-openapi.yml
  format: yaml
  label: King Fahd University of Petroleum & Minerals Oai Pmh API
  slug: kfupm-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-oai-pmh-api-openapi.yml
- filename: kfupm-search-api-openapi.yml
  format: yaml
  label: King Fahd University of Petroleum & Minerals Search API
  slug: kfupm-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-search-api-openapi.yml
- filename: kfupm-oauth2-api-openapi.yml
  format: yaml
  label: King Fahd University of Petroleum & Minerals Oauth2 API
  slug: kfupm-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-oauth2-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by KFUPM's own identity provider. Read verbatim from `scopes_supported` in the institution's OIDC discovery document. These are the AD FS built-in scope set; KFUPM has not published any application-specific scope beyond it, and no public client-registration path was found.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kfupm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'King Fahd University of Petroleum & Minerals publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the King Fahd University of Petroleum & Minerals API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: King Fahd University of Petroleum & Minerals
provider_slug: kfupm
schemes: []
scope_count: 9
scope_names:
- openid
- profile
- email
- allatclaims
- user_impersonation
- logon_cert
- vpn_cert
- winhello_cert
- aza
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope; requests profile claims.
  flows: []
  scope: profile
- description: Standard OIDC scope; requests the email claim.
  flows: []
  scope: email
- description: AD FS scope requesting that all claims be included in the access token.
  flows: []
  scope: allatclaims
- description: AD FS scope permitting a relying party to act on behalf of the signed-in user.
  flows: []
  scope: user_impersonation
- description: AD FS scope issuing a logon certificate.
  flows: []
  scope: logon_cert
- description: AD FS scope issuing a VPN certificate.
  flows: []
  scope: vpn_cert
- description: AD FS scope issuing a Windows Hello for Business certificate.
  flows: []
  scope: winhello_cert
- description: AD FS scope used for the primary refresh / brokered authentication flow.
  flows: []
  scope: aza
slug: kfupm-scopes
source_filename: kfupm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration (200, 2026-08-30)\nprovider: King Fahd University of Petroleum & Minerals\nproviderId: kfupm\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by KFUPM's own identity provider. Read verbatim\n  from `scopes_supported` in the institution's OIDC discovery document. These are the AD FS\n  built-in scope set; KFUPM has not published any application-specific scope beyond it, and no\n  public client-registration path was found.\nx-operator: institution\nissuer: https://sts.kfupm.edu.sa/adfs\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n  - name: profile\n    description: Standard OIDC scope; requests profile claims.\n  - name: email\n    description: Standard OIDC scope; requests the email claim.\n  - name: allatclaims\n    description: AD FS scope requesting that all claims be included in the access token.\n\
  \  - name: user_impersonation\n    description: AD FS scope permitting a relying party to act on behalf of the signed-in user.\n  - name: logon_cert\n    description: AD FS scope issuing a logon certificate.\n  - name: vpn_cert\n    description: AD FS scope issuing a VPN certificate.\n  - name: winhello_cert\n    description: AD FS scope issuing a Windows Hello for Business certificate.\n  - name: aza\n    description: AD FS scope used for the primary refresh / brokered authentication flow.\nclaims_supported:\n  [aud, iss, iat, exp, auth_time, nonce, at_hash, c_hash, sub, upn, unique_name, pwd_url,\n   pwd_exp, mfa_auth_time, sid, nbf]\nnotes: >-\n  No scope here is application-specific. KFUPM publishes no developer portal, no client\n  registration endpoint and no scope documentation; a relying party is onboarded by KFUPM IT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/scopes/kfupm-scopes.yml
summary_line: 9 scopes
tags:
- University
- Higher Education
- Education
- Research
- Saudi Arabia
- Middle East
- Identity Federation
- Research Repository
- Open Access
- OAI-PMH
- Theses
- Course Catalog
token_bound: false
token_urls: []
---
