---
api_specs:
- filename: kfupm-identity-federation-openapi.yml
  format: yaml
  label: KFUPM Identity Federation (SAML 2.0 + OpenID Connect)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-identity-federation-openapi.yml
- filename: kfupm-eprints-oai-pmh-openapi.yml
  format: yaml
  label: KFUPM ePrints OAI-PMH Repository Interface
  slug: eprints-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-eprints-oai-pmh-openapi.yml
- filename: kfupm-eprints-export-openapi.yml
  format: yaml
  label: KFUPM ePrints Export & Search (JSON)
  slug: eprints-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-eprints-export-openapi.yml
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
overview: 'King Fahd University of Petroleum & Minerals uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: King Fahd University of Petroleum & Minerals
provider_slug: kfupm
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kfupm-scopes
source_filename: kfupm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration (200, 2026-08-30)\nprovider: King Fahd University of Petroleum & Minerals\nproviderId: kfupm\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by KFUPM's own identity provider. Read verbatim\n  from `scopes_supported` in the institution's OIDC discovery document. These are the AD FS\n  built-in scope set; KFUPM has not published any application-specific scope beyond it, and no\n  public client-registration path was found.\nx-operator: institution\nissuer: https://sts.kfupm.edu.sa/adfs\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n  - name: profile\n    description: Standard OIDC scope; requests profile claims.\n  - name: email\n    description: Standard OIDC scope; requests the email claim.\n  - name: allatclaims\n    description: AD FS scope requesting that all claims be included in the access token.\n\
  \  - name: user_impersonation\n    description: AD FS scope permitting a relying party to act on behalf of the signed-in user.\n  - name: logon_cert\n    description: AD FS scope issuing a logon certificate.\n  - name: vpn_cert\n    description: AD FS scope issuing a VPN certificate.\n  - name: winhello_cert\n    description: AD FS scope issuing a Windows Hello for Business certificate.\n  - name: aza\n    description: AD FS scope used for the primary refresh / brokered authentication flow.\nclaims_supported:\n  [aud, iss, iat, exp, auth_time, nonce, at_hash, c_hash, sub, upn, unique_name, pwd_url,\n   pwd_exp, mfa_auth_time, sid, nbf]\nnotes: >-\n  No scope here is application-specific. KFUPM publishes no developer portal, no client\n  registration endpoint and no scope documentation; a relying party is onboarded by KFUPM IT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/scopes/kfupm-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
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
token_urls: []
---
