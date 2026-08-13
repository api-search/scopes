---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Darrow Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes advertised by Darrow''s Auth0 identity tenant, read from `scopes_supported` in its OpenID Connect discovery document. They are the standard OIDC/Auth0 profile scopes — Darrow publishes no product API and therefore no API-specific permission scopes. Absence of custom scopes here is a finding, not a gap in the probe: no public resource-server metadata or scope reference exists.'
overview: 'Darrow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Darrow
provider_slug: darrow
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: darrow-scopes
source_filename: darrow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://auth.darrow.ai/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes advertised by Darrow's Auth0 identity tenant, read from\n  `scopes_supported` in its OpenID Connect discovery document. They are the standard\n  OIDC/Auth0 profile scopes — Darrow publishes no product API and therefore no\n  API-specific permission scopes. Absence of custom scopes here is a finding, not a gap\n  in the probe: no public resource-server metadata or scope reference exists.\nissuer: https://auth.darrow.ai/\nscope_count: 14\ncustom_scope_count: 0\nscopes:\n- name: openid\n  description: Request an ID token (OIDC core).\n  standard: oidc\n- name: profile\n  description: Basic profile claims (name, family_name, given_name, nickname, picture, created_at).\n  standard: oidc\n- name: offline_access\n  description: Issue a refresh token for long-lived access.\n  standard: oidc\n- name: email\n  description: Email address\
  \ claim.\n  standard: oidc\n- name: email_verified\n  description: Email verification status claim.\n  standard: auth0\n- name: address\n  description: Address claim.\n  standard: oidc\n- name: phone\n  description: Phone number claim.\n  standard: oidc\n- name: name\n  description: Full name claim.\n  standard: auth0\n- name: given_name\n  description: Given name claim.\n  standard: auth0\n- name: family_name\n  description: Family name claim.\n  standard: auth0\n- name: nickname\n  description: Nickname claim.\n  standard: auth0\n- name: picture\n  description: Profile picture URL claim.\n  standard: auth0\n- name: created_at\n  description: Account creation timestamp claim.\n  standard: auth0\n- name: identities\n  description: Linked identity provider records.\n  standard: auth0\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://auth.darrow.ai/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darrow/refs/heads/main/scopes/darrow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Legal
- Legal Intelligence
- Litigation
- Artificial Intelligence
- Compliance
- Risk Management
- Insurance
- Data Analytics
token_urls: []
---
