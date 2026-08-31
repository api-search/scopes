---
api_specs:
- filename: ustc-campus-status-api-openapi.yml
  format: yaml
  label: USTC Campus Enrollment Status Query API (在校状态查询接口)
  slug: campus-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ustc/refs/heads/main/openapi/ustc-campus-status-api-openapi.yml
authorization_urls: []
description: The authorization scopes USTC's unified identity authorization server advertises, and the claims it says it can release. Institution-operated. Scope here governs access to personal attributes of campus members rather than to a data API — this is an identity provider, not a data platform, and the scope list is the only published authorization vocabulary the institution has.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ustc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Science and Technology of China uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Science and Technology of China
provider_slug: ustc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ustc-scopes
source_filename: ustc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Evangelist Scopes\nspecificationVersion: '0.1'\nprovider: University of Science and Technology of China\nproviderId: ustc\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration (200, fetched 2026-08-30) —\n  `scopes_supported` and `claims_supported` read verbatim from the live discovery document; and\n  https://id.ustc.edu.cn/doc/developer/ (200) — the OAuth 2.0 scope parameter table in USTC's\n  own developer manual.\ndescription: >-\n  The authorization scopes USTC's unified identity authorization server advertises, and the\n  claims it says it can release. Institution-operated. Scope here governs access to personal\n  attributes of campus members rather than to a data API — this is an identity provider, not a\n  data platform, and the scope list is the only published authorization vocabulary the\n  institution has.\nx-operator: institution\n\noidc_scopes:\n- name: openid\n  required: true\n\
  \  description: Base OpenID Connect scope; requests an ID token.\n- name: profile\n  description: Standard OIDC profile claims.\n- name: email\n  description: email, email_verified.\n- name: address\n  description: Postal address claim.\n- name: phone\n  description: phone_number, phone_number_verified.\n- name: offline_access\n  description: Requests a refresh token.\n\noauth2_documented_scopes:\n- name: gid\n  description: 人员全局标识 — the campus global person identifier.\n- name: email\n  description: Campus email address.\n- name: name\n  description: Display name.\nnote_on_oauth2_scopes: >-\n  USTC's developer manual marks `scope` OPTIONAL and states that in normal use it is not sent:\n  for CAS compatibility, the attribute set released to an application is configured per\n  registered client and returned from the profile endpoint. Authorization is therefore\n  administrator-configured rather than caller-requested — a real property of this deployment,\n  not an omission in the documentation.\n\
  \nclaims_supported:\n- sub\n- name\n- preferred_username\n- family_name\n- given_name\n- middle_name\n- profile\n- picture\n- nickname\n- website\n- zoneinfo\n- locale\n- updated_at\n- birthdate\n- email\n- email_verified\n- phone_number\n- phone_number_verified\n- address\n- gender\n\nobservations:\n- >-\n  `given_name` appears twice in the live `claims_supported` array. Harmless, but it is a\n  hand-edited configuration artifact rather than a generated one.\n- >-\n  The advertised claim set includes birthdate, gender, phone_number and address — direct\n  personal data about students and staff. Combined with an administrator-configured release\n  policy and no public client registration, the practical control on that data is the manual\n  onboarding process, which USTC documents and restricts to on-campus applications.\n- >-\n  The enrollment status API at /doc/api/ has no scope model at all: a token either carries\n  access or it does not, and the second control is the source-IP allowlist.\
  \ Its documented\n  design deliberately returns only a status code rather than a person record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ustc/refs/heads/main/scopes/ustc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- China
- C9 League
- Chinese Academy of Sciences
- Research
- Identity Federation
- Single Sign-On
- Course Catalog
- Research Computing
- Open Source Mirror
token_urls: []
---
