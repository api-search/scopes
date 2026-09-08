---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Electronic Arts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Electronic Arts uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Electronic Arts
provider_slug: electronic-arts
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: electronic-arts-scopes
source_filename: electronic-arts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  scopes_supported in https://accounts.ea.com/.well-known/openid-configuration (HTTP 200,\n  fetched 2026-09-06, saved verbatim to well-known/electronic-arts-openid-configuration.json).\n  No scope reference page is published by EA; searched www.ea.com, help.ea.com and the FC\n  Community API announcement and none exists.\nprovider: Electronic Arts\nproviderId: electronic-arts\nauthorization_server: https://accounts.ea.com/connect/auth\nscope_count: 4\nscopes:\n- name: openid\n  description: >-\n    OpenID Connect authentication. Required to receive an RS256-signed ID token from\n    accounts.ea.com. Description is the OIDC Core 1.0 definition; EA publishes none of its own.\n  source: discovery document\n- name: email\n  description: >-\n    Releases the email and email_verified claims, both of which are listed in\n    claims_supported.\n  source: discovery document\n- name: phone\n  description: >-\n    Releases the phone_number\
  \ and phone_number_verified claims, both listed in\n    claims_supported.\n  source: discovery document\n- name: profile\n  description: >-\n    Releases the profile claims EA lists in claims_supported: name, given_name, family_name,\n    gender, locale and auth_time.\n  source: discovery document\nclaims_supported:\n- sub\n- aud\n- exp\n- iat\n- iss\n- email\n- email_verified\n- family_name\n- given_name\n- gender\n- auth_time\n- locale\n- name\n- phone_number\n- phone_number_verified\n- c_hash\n- at_hash\nnotes:\n- >-\n  These four are the IDENTITY scopes only. The EA SPORTS FC Community API grants partners\n  permission to read Ultimate Team data — \"players, formations, tactics, and more\" in EA's\n  own words — and whatever scope strings carry that grant are NOT published in the discovery\n  document or anywhere else on EA's public surface.\n- >-\n  A consent screen exists (EA: \"You'll be asked to grant that website permission to make\n  specific requests to FC services on your behalf\"\
  ) but its scope labels are visible only\n  to approved partners' users.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electronic-arts/refs/heads/main/scopes/electronic-arts-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Gaming
- Video Games
- Entertainment
- Consumer
- Player Services
- Fortune 1000
token_urls: []
---
