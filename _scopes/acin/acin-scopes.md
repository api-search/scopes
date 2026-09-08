---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Acin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Acin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acin
provider_slug: acin
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: acin-scopes
source_filename: acin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  scopes_supported in https://app-auth.acin.com/.well-known/openid-configuration (HTTP 200,\n  fetched anonymously 2026-09-06). Acin publishes no OpenAPI and no scopes/permissions reference\n  page, so these are the identity scopes the authorization server advertises — NOT the API\n  permission scopes the apim-prod.acin.com gateway enforces, which are not published anywhere\n  public.\nauthorization_server: https://app-auth.acin.com/\ndocs: null\nscope_count: 14\nscopes:\n- name: openid\n  description: OIDC — request an ID token.\n  standard: true\n- name: profile\n  description: OIDC standard claim set for the end user's profile.\n  standard: true\n- name: offline_access\n  description: OIDC — request a refresh token.\n  standard: true\n- name: email\n  description: OIDC standard claim — the user's email address.\n  standard: true\n- name: email_verified\n  description: OIDC standard claim — whether the email address is\
  \ verified.\n  standard: true\n- name: name\n  description: OIDC standard claim — full name.\n  standard: true\n- name: given_name\n  description: OIDC standard claim — given name.\n  standard: true\n- name: family_name\n  description: OIDC standard claim — family name.\n  standard: true\n- name: nickname\n  description: OIDC standard claim — nickname.\n  standard: true\n- name: picture\n  description: OIDC standard claim — profile picture URL.\n  standard: true\n- name: phone\n  description: OIDC standard claim — phone number.\n  standard: true\n- name: address\n  description: OIDC standard claim — postal address.\n  standard: true\n- name: created_at\n  description: Auth0 tenant claim — account creation timestamp.\n  standard: false\n- name: identities\n  description: Auth0 tenant claim — linked identity providers for the user.\n  standard: false\ngaps:\n- >-\n  No API-permission scopes are published. The GraphQL gateway at apim-prod.acin.com rejects\n  anonymous requests with HTTP 401,\
  \ so the audience and scope values a client would request cannot\n  be observed without a tenant credential.\n- No scopes or permissions reference page exists on any public Acin surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acin/refs/heads/main/scopes/acin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Operational Risk
- Risk Management
- Non-Financial Risk
- Financial Services
- Banking
- Compliance
- Regulatory Technology
- Benchmarking
- Data Standards
token_urls: []
---
