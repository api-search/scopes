---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Meow Wolf Scopes
name_suffix: OAuth Scopes
note: Meow Wolf publishes no scope or permission reference — there is no developer documentation of any kind. Every scope below is read verbatim from scopes_supported in the live OIDC discovery document served by the company's Auth0 custom-domain tenant. They are the stock OpenID Connect identity scopes plus Auth0's per-claim scopes; NONE of them grants access to a Meow Wolf business API, because no such API is published. Descriptions are the standard OIDC Core 1.0 / Auth0 meanings, not vendor-authored text.
overview: 'Meow Wolf uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meow Wolf
provider_slug: meow-wolf
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: meow-wolf-scopes
source_filename: meow-wolf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://auth.meowwolf.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Meow Wolf publishes no scope or permission reference — there is no developer\n  documentation of any kind. Every scope below is read verbatim from scopes_supported in\n  the live OIDC discovery document served by the company's Auth0 custom-domain tenant.\n  They are the stock OpenID Connect identity scopes plus Auth0's per-claim scopes; NONE\n  of them grants access to a Meow Wolf business API, because no such API is published.\n  Descriptions are the standard OIDC Core 1.0 / Auth0 meanings, not vendor-authored text.\nscope_count: 14\nscopes:\n- name: openid\n  description: Required to obtain an ID token and use OpenID Connect at all.\n- name: profile\n  description: Requests the default profile claims (name, family_name, given_name, nickname, picture, updated_at).\n- name: offline_access\n  description: Requests a refresh token so the client\
  \ can renew access without user interaction.\n- name: email\n  description: Requests the email claim.\n- name: email_verified\n  description: Requests the email_verified claim.\n- name: name\n  description: Requests the full name claim.\n- name: given_name\n  description: Requests the given name claim.\n- name: family_name\n  description: Requests the family name claim.\n- name: nickname\n  description: Requests the nickname claim.\n- name: picture\n  description: Requests the profile picture URL claim.\n- name: phone\n  description: Requests the phone_number claim.\n- name: address\n  description: Requests the address claim.\n- name: created_at\n  description: Auth0 claim — account creation timestamp.\n- name: identities\n  description: Auth0 claim — the linked identity-provider identities for the user.\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n\
  - sub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow-wolf/refs/heads/main/scopes/meow-wolf-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Art
- Entertainment
- Immersive Experiences
- Events
- Ticketing
- Museums
- Tourism
- Retail
- Mobile Apps
token_urls: []
---
