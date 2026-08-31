---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ianacare Scopes
name_suffix: OAuth Scopes
note: These are the scopes ianacare's own authorization server advertises in its discovery document. They are the standard OIDC/Auth0 identity scope set — ianacare publishes no API-specific permission scopes anywhere public, and no audience/API identifier is discoverable, so no resource scopes could be recorded. Nothing here was authored; every entry is copied from scopes_supported.
overview: 'ianacare uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ianacare
provider_slug: ianacare
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ianacare-scopes
source_filename: ianacare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.ianacare.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes ianacare's own authorization server advertises in its discovery\n  document. They are the standard OIDC/Auth0 identity scope set — ianacare publishes no\n  API-specific permission scopes anywhere public, and no audience/API identifier is\n  discoverable, so no resource scopes could be recorded. Nothing here was authored;\n  every entry is copied from scopes_supported.\ndocs: null\nauthorization_server: https://auth.ianacare.com/\nscope_count: 14\nscopes:\n- name: openid\n  description: Request an ID token — the OpenID Connect entry scope.\n- name: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture).\n- name: offline_access\n  description: Issue a refresh token so the client can renew access without re-prompting.\n- name: name\n  description: The end user's full name claim.\n- name: given_name\n\
  \  description: The end user's given name claim.\n- name: family_name\n  description: The end user's family name claim.\n- name: nickname\n  description: The end user's nickname claim.\n- name: email\n  description: The end user's email address claim.\n- name: email_verified\n  description: Whether the end user's email address has been verified.\n- name: picture\n  description: URL of the end user's profile picture.\n- name: created_at\n  description: Account creation timestamp claim.\n- name: identities\n  description: Linked identity-provider identities for the account.\n- name: phone\n  description: The end user's phone number claims.\n- name: address\n  description: The end user's address claims.\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\ngaps:\n- No resource/API scopes published (no audience identifier is discoverable anonymously).\n\
  - No scopes or permissions reference page exists on any ianacare host.\nx-evidence:\n  fetched: '2026-08-22'\n  urls:\n  - url: https://auth.ianacare.com/.well-known/openid-configuration\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ianacare/refs/heads/main/scopes/ianacare-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Caregiving
- Employee Benefits
- Digital Health
- Care Navigation
- Health Plans
- Mobile Application
- Identity
token_urls: []
---
