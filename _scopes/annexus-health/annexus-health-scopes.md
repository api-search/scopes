---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Annexus Health Scopes
name_suffix: OAuth Scopes
note: These are the scopes the AssistPoint production authorization server advertises in its anonymous OpenID Connect discovery document. They are the standard OIDC profile set — no AssistPoint or AP Connect resource-level scopes are published. Any partner-facing API scopes are issued privately as part of an AP Connect integration agreement and were not fabricated here.
overview: 'Annexus Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Annexus Health
provider_slug: annexus-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: annexus-health-scopes
source_filename: annexus-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://login.live.annexushealth.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes the AssistPoint production authorization server advertises in its\n  anonymous OpenID Connect discovery document. They are the standard OIDC profile set — no\n  AssistPoint or AP Connect resource-level scopes are published. Any partner-facing API scopes\n  are issued privately as part of an AP Connect integration agreement and were not fabricated\n  here.\nissuer: https://login.live.annexushealth.com/\nscheme: assistpoint_oidc\nscopes:\n- name: openid\n  description: Required to request an ID token and initiate an OpenID Connect flow.\n  standard: openid-connect-core-1.0\n- name: profile\n  description: Default profile claims — name, family_name, given_name, nickname, picture, updated_at.\n  standard: openid-connect-core-1.0\n- name: offline_access\n  description: Issues a refresh token so the client can obtain new access\
  \ tokens without user interaction.\n  standard: openid-connect-core-1.0\n- name: name\n  description: The end-user's full display name.\n- name: given_name\n  description: The end-user's given (first) name.\n- name: family_name\n  description: The end-user's family (last) name.\n- name: nickname\n  description: The end-user's casual or short name.\n- name: email\n  description: The end-user's preferred email address.\n  standard: openid-connect-core-1.0\n- name: email_verified\n  description: Boolean indicating whether the end-user's email address has been verified.\n- name: picture\n  description: URL of the end-user's profile picture.\n- name: created_at\n  description: Timestamp the end-user's identity record was created.\n- name: identities\n  description: The linked identity provider records associated with the end-user.\n- name: phone\n  description: The end-user's phone number and phone_number_verified claim.\n  standard: openid-connect-core-1.0\n- name: address\n  description:\
  \ The end-user's postal address claim.\n  standard: openid-connect-core-1.0\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://login.live.annexushealth.com/.well-known/openid-configuration\n  http_status: 200\n  field: scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/annexus-health/refs/heads/main/scopes/annexus-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Health Technology
- Patient Access
- Financial Assistance
- Oncology
- Revenue Cycle
- Copay Assistance
- Identity
- OpenID Connect
- HITRUST
token_urls: []
---
