---
authorization_urls: []
description: RapidDeploy publishes no scopes/permissions reference. The scopes below are the scopes_supported array advertised by the company's own Auth0 tenant discovery document - they are the standard OIDC identity scopes plus offline_access, and are NOT API authorization scopes. Any API-level scope surface for api.rapiddeploy.com is defined per-tenant inside the Auth0 API registration and is not anonymously discoverable.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rapiddeploy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RapidDeploy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RapidDeploy
provider_slug: rapiddeploy
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rapiddeploy-scopes
source_filename: rapiddeploy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://auth.rapiddeploy.com/.well-known/openid-configuration\ndocs: null\nname: RapidDeploy OAuth scopes\ndescription: >-\n  RapidDeploy publishes no scopes/permissions reference. The scopes below are the\n  scopes_supported array advertised by the company's own Auth0 tenant discovery document - they are\n  the standard OIDC identity scopes plus offline_access, and are NOT API authorization scopes. Any\n  API-level scope surface for api.rapiddeploy.com is defined per-tenant inside the Auth0 API\n  registration and is not anonymously discoverable.\nissuer: https://auth.rapiddeploy.com/\nscope_count: 14\nscopes:\n- name: openid\n  description: 'OIDC: request an ID token.'\n  standard: true\n- name: profile\n  description: 'OIDC: basic profile claims.'\n  standard: true\n- name: offline_access\n  description: 'OIDC: issue a refresh token.'\n  standard: true\n- name: name\n  description: 'Identity claim: full name.'\n  standard:\
  \ true\n- name: given_name\n  description: 'Identity claim: given name.'\n  standard: true\n- name: family_name\n  description: 'Identity claim: family name.'\n  standard: true\n- name: nickname\n  description: 'Identity claim: nickname.'\n  standard: true\n- name: email\n  description: 'Identity claim: email address.'\n  standard: true\n- name: email_verified\n  description: 'Identity claim: email verification state.'\n  standard: true\n- name: picture\n  description: 'Identity claim: profile picture URL.'\n  standard: true\n- name: created_at\n  description: 'Identity claim: account creation time.'\n  standard: true\n- name: identities\n  description: 'Identity claim: linked identity providers.'\n  standard: true\n- name: phone\n  description: 'Identity claim: phone number.'\n  standard: true\n- name: address\n  description: 'Identity claim: address.'\n  standard: true\napi_scopes: []\napi_scopes_note: >-\n  None published. Determining the authorization scopes that gate RapidDeploy platform\
  \ operations\n  requires an issued tenant client; they cannot be read anonymously.\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://auth.rapiddeploy.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapiddeploy/refs/heads/main/scopes/rapiddeploy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Public Safety
- Emergency Services
- NG911
- Computer-Aided Dispatch
- Mapping
- Analytics
- Government
- Cloud
token_urls: []
---
