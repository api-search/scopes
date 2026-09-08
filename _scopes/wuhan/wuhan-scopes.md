---
authorization_urls: []
description: The only scope vocabulary Wuhan University publishes anywhere. These are the standard OpenID Connect 1.0 scopes as emitted by the Wisedu CAS authorization server at cas.whu.edu.cn; there are no institution-specific scopes, no resource scopes, and no data-API scopes, because there is no institution-operated data API to scope. Scopes here govern who may read a WHU identity, not what a client may do with WHU information.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Wuhan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wuhan University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wuhan University
provider_slug: wuhan
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wuhan-scopes
source_filename: wuhan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Evangelist Scopes\nspecificationVersion: '0.1'\nprovider: Wuhan University\nproviderId: wuhan\ngenerated: '2026-09-01'\nmethod: searched\nsource: >-\n  scopes_supported and claims_supported read verbatim from the OpenID Connect discovery document\n  Wuhan University publishes at\n  https://cas.whu.edu.cn/authserver/oidc/.well-known/openid-configuration (HTTP 200,\n  application/json;charset=UTF-8, 1,340 bytes, fetched 2026-09-01, archived at\n  authentication/wuhan-cas-oidc-openid-configuration.json). Nothing in this file is inferred or\n  generated -- every value below appears in that document.\ndescription: >-\n  The only scope vocabulary Wuhan University publishes anywhere. These are the standard OpenID\n  Connect 1.0 scopes as emitted by the Wisedu CAS authorization server at cas.whu.edu.cn; there\n  are no institution-specific scopes, no resource scopes, and no data-API scopes, because there\n  is no institution-operated data API to scope. Scopes here\
  \ govern who may read a WHU identity,\n  not what a client may do with WHU information.\n\nx-operator: institution\nx-operator-basis: >-\n  Served from cas.whu.edu.cn (115.156.123.25, netname WHR-CERNET, Wuhan Regional Network). The\n  scope SET is the OIDC standard as shipped by the supplier's product, not a WHU design -- the\n  deployment is institution-operated, the vocabulary is the specification's.\n\nissuer: https://cas.whu.edu.cn/authserver/oidc/\n\nscopes:\n- name: openid\n  standard: OpenID Connect Core 1.0\n  description: Required to request an ID token; identifies the request as an OIDC authentication.\n- name: profile\n  standard: OpenID Connect Core 1.0\n  description: >-\n    Releases the profile claim set the server advertises: name, preferred_username, family_name,\n    given_name, middle_name, nickname, picture, website, gender, birthdate, zoneinfo, locale,\n    updated_at.\n- name: email\n  standard: OpenID Connect Core 1.0\n  description: Releases email and email_verified.\n\
  - name: address\n  standard: OpenID Connect Core 1.0\n  description: Releases the address claim.\n- name: phone\n  standard: OpenID Connect Core 1.0\n  description: Releases phone_number and phone_number_verified.\n- name: offline_access\n  standard: OpenID Connect Core 1.0\n  description: Requests a refresh token for use when the subject is not present.\n\nclaims_supported:\n- sub\n- name\n- preferred_username\n- family_name\n- given_name\n- middle_name\n- profile\n- picture\n- nickname\n- website\n- zoneinfo\n- locale\n- updated_at\n- birthdate\n- email\n- email_verified\n- phone_number\n- phone_number_verified\n- address\n- gender\n\nobservations:\n- >-\n  claims_supported lists given_name twice. A duplicate entry in a published discovery document\n  is a small correctness defect in the artifact, and it is reproduced faithfully above minus the\n  duplicate.\n- >-\n  No institution-defined scope exists. Every scope is the OIDC standard set, which is the\n  expected shape for a campus\
  \ SSO and the expected absence for an institution that operates no\n  public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wuhan/refs/heads/main/scopes/wuhan-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Research
- China
- Identity Federation
- Single Sign-On
- Research Data
- GNSS
- Library
- Open-Source
token_urls: []
---
