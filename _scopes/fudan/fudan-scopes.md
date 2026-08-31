---
api_specs:
- filename: fudan-identity-openapi.yml
  format: yaml
  label: Fudan University Unified Identity — OpenID Connect
  slug: identity-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/openapi/fudan-identity-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fudan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fudan University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fudan University
provider_slug: fudan
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fudan-scopes
source_filename: fudan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "x-method: derived\nname: Fudan University — declared scopes\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://id.fudan.edu.cn/idp/.well-known/openid-configuration\nx-operator: institution\nsummary: >-\n  The only authorization scope Fudan University declares anywhere machine-readable is the\n  mandatory OpenID Connect scope. There is no scoped API programme, and no other surface\n  in this repository publishes a scope vocabulary.\nscopes:\n  - name: openid\n    surface: Fudan University OpenID Connect provider\n    description: >-\n      Mandatory OpenID Connect scope. The only member of scopes_supported in the live\n      discovery document; no profile, email or institution-specific scope is offered.\n    evidence:\n      url: https://id.fudan.edu.cn/idp/.well-known/openid-configuration\n      status: 200\n      location: scopes_supported\nclaims:\n  note: >-\n    claims_supported in the same document, recorded here because Fudan exposes no scope\n    beyond openid\
  \ and the claim list is the only released-attribute signal available.\n  values: [ sub, iss, auth_time, aud, exp, iat, uid ]\nnot_found:\n  - Any scope vocabulary for the research data platform at rdr.fudan.edu.cn.\n  - Any SAML attribute-release policy published alongside the IdP metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/scopes/fudan-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- China
- Shanghai
- C9 League
- Identity Federation
- Research Data
- Single Sign-On
token_urls: []
---
