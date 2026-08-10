---
authorization_urls: []
description: The only OAuth scopes BEKhealth publishes anonymously are the standard OpenID Connect scopes and claim-scopes advertised by its Auth0 issuer's discovery document. These govern identity for the customer application and the gated documentation portal. BEKhealth advertises NO product or API scopes — no resource-server audience is published, and there is no public scopes or permissions reference page to search. Everything below is taken verbatim from `scopes_supported`; nothing has been inferred or invented.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Bekhealth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BEKHealth uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BEKHealth
provider_slug: bekhealth
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bekhealth-scopes
source_filename: bekhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.bekhealth.com/.well-known/openid-configuration\ndescription: >-\n  The only OAuth scopes BEKhealth publishes anonymously are the standard OpenID\n  Connect scopes and claim-scopes advertised by its Auth0 issuer's discovery\n  document. These govern identity for the customer application and the gated\n  documentation portal. BEKhealth advertises NO product or API scopes — no\n  resource-server audience is published, and there is no public scopes or\n  permissions reference page to search. Everything below is taken verbatim from\n  `scopes_supported`; nothing has been inferred or invented.\nissuer: https://auth.bekhealth.com/\ndocs: null\ndocs_note: No public scopes / permissions reference page exists on any BEKhealth host.\nscope_source: openid-configuration.scopes_supported\nscopes:\n- name: openid\n  standard: OpenID Connect Core 1.0\n  description: Requests an ID Token; required for any OIDC authentication request.\n\
  - name: profile\n  standard: OpenID Connect Core 1.0\n  description: Requests the default profile claims (name, family_name, given_name, nickname, picture).\n- name: offline_access\n  standard: OpenID Connect Core 1.0\n  description: Requests a refresh token so the client can renew access without user interaction.\n- name: email\n  standard: OpenID Connect Core 1.0\n  description: Requests the email claim.\n- name: email_verified\n  standard: Auth0 claim scope\n  description: Requests the email_verified claim.\n- name: name\n  standard: Auth0 claim scope\n  description: Requests the name claim.\n- name: given_name\n  standard: Auth0 claim scope\n  description: Requests the given_name claim.\n- name: family_name\n  standard: Auth0 claim scope\n  description: Requests the family_name claim.\n- name: nickname\n  standard: Auth0 claim scope\n  description: Requests the nickname claim.\n- name: picture\n  standard: Auth0 claim scope\n  description: Requests the picture claim.\n- name: created_at\n\
  \  standard: Auth0 claim scope\n  description: Requests the created_at claim (account creation timestamp).\n- name: identities\n  standard: Auth0 claim scope\n  description: Requests the identities claim (linked identity-provider accounts).\n- name: phone\n  standard: OpenID Connect Core 1.0\n  description: Requests the phone_number claim.\n- name: address\n  standard: OpenID Connect Core 1.0\n  description: Requests the address claim.\nobserved_in_use:\n- scope: openid\n  where: docs.bekhealth.com login redirect\n- scope: email\n  where: docs.bekhealth.com login redirect\ncoverage:\n  identity_scopes: 14\n  api_scopes: 0\n  note: >-\n    Zero API/product scopes are published. An integrator cannot determine from\n    any public artifact what a BEKhealth access token would be authorized to do.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://auth.bekhealth.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://docs.bekhealth.com/\n    http_status:\
  \ 302\n    note: 'redirect carries scope=openid%20email'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bekhealth/refs/heads/main/scopes/bekhealth-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Clinical Trials
- Clinical Research
- Electronic Health Records
- Real World Data
- Artificial Intelligence
- Patient Recruitment
- Life Sciences
- Health Data
token_urls: []
---
