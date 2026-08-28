---
authorization_urls: []
description: The complete scopes_supported list published by the OncoLens authorization server at login.oncolens.com. These are OpenID Connect standard and Auth0 profile-claim scopes for the sign-in flow — they are identity scopes, not product-resource scopes. OncoLens publishes no API resource scopes (no read:cases, write:tumor_board or similar), because it publishes no API. No scopes reference PHI, patient records, tumor boards, registry data or clinical trials.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Oncolens Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OncoLens uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OncoLens
provider_slug: oncolens
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: oncolens-scopes
source_filename: oncolens-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://login.oncolens.com/.well-known/openid-configuration\nname: OncoLens OAuth / OIDC scopes\ndescription: >-\n  The complete scopes_supported list published by the OncoLens authorization server at\n  login.oncolens.com. These are OpenID Connect standard and Auth0 profile-claim scopes for\n  the sign-in flow — they are identity scopes, not product-resource scopes. OncoLens\n  publishes no API resource scopes (no read:cases, write:tumor_board or similar), because it\n  publishes no API. No scopes reference PHI, patient records, tumor boards, registry data or\n  clinical trials.\ndocs: null\ndocs_note: >-\n  OncoLens publishes no scope reference or permissions documentation page. The list below is\n  read directly from the machine-readable discovery document, which is the only published\n  source.\nauthorization_server: https://login.oncolens.com/\nscope_count: 14\nresource_scope_count: 0\nscopes:\n- name: openid\n  description:\
  \ Required to issue an ID token; signals an OpenID Connect request.\n  standard: OpenID Connect Core 1.0\n- name: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture, updated_at).\n  standard: OpenID Connect Core 1.0\n- name: email\n  description: The end user's email address claim.\n  standard: OpenID Connect Core 1.0\n- name: email_verified\n  description: Whether the end user's email address has been verified.\n  standard: Auth0 profile claim\n- name: address\n  description: The end user's postal address claim.\n  standard: OpenID Connect Core 1.0\n- name: phone\n  description: The end user's phone number and verification status.\n  standard: OpenID Connect Core 1.0\n- name: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens without the user present.\n  standard: OpenID Connect Core 1.0\n- name: name\n  description: Full display name claim.\n  standard: Auth0 profile claim\n- name: given_name\n\
  \  description: First name claim.\n  standard: Auth0 profile claim\n- name: family_name\n  description: Last name claim.\n  standard: Auth0 profile claim\n- name: nickname\n  description: Nickname / short display name claim.\n  standard: Auth0 profile claim\n- name: picture\n  description: Profile picture URL claim.\n  standard: Auth0 profile claim\n- name: created_at\n  description: Account creation timestamp claim.\n  standard: Auth0 profile claim\n- name: identities\n  description: Linked identity-provider connections for the account.\n  standard: Auth0 profile claim\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oncolens/refs/heads/main/scopes/oncolens-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Oncology
- Cancer Care
- Clinical Trials
- Health Data
- Real World Data
- Artificial Intelligence
- Analytics
- Clinical Workflow
- Cancer Registry
- Life Sciences
- SaaS
token_urls: []
---
