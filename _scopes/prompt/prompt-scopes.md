---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Prompt Scopes
name_suffix: OAuth Scopes
note: These are the scopes the Prompt identity provider advertises in `scopes_supported`. They are the standard OpenID Connect scopes and OIDC standard-claim scopes only — Prompt publishes no product/API permission scopes anywhere public, because it publishes no public API reference. Do not read this file as an authorization model for a Prompt product API; it is the login surface.
overview: 'Prompt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prompt
provider_slug: prompt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: prompt-scopes
source_filename: prompt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://authenticate.promptemr.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes the Prompt identity provider advertises in `scopes_supported`. They are the\n  standard OpenID Connect scopes and OIDC standard-claim scopes only — Prompt publishes no\n  product/API permission scopes anywhere public, because it publishes no public API reference. Do\n  not read this file as an authorization model for a Prompt product API; it is the login surface.\nauthorization_server: https://authenticate.promptemr.com/\nscope_count: 14\nscopes:\n- name: openid\n  description: Required OIDC scope; requests an ID token for the authenticated user.\n  standard: openid-connect-core\n- name: profile\n  description: Requests the OIDC standard profile claims.\n  standard: openid-connect-core\n- name: offline_access\n  description: Requests a refresh token for long-lived access.\n  standard: openid-connect-core\n- name: email\n  description:\
  \ Requests the user's email address claim.\n  standard: openid-connect-core\n- name: email_verified\n  description: Requests the email verification status claim.\n  standard: openid-connect-core\n- name: address\n  description: Requests the OIDC standard address claim.\n  standard: openid-connect-core\n- name: phone\n  description: Requests the OIDC standard phone claims.\n  standard: openid-connect-core\n- name: name\n  description: Requests the user's full name claim.\n  standard: openid-connect-core\n- name: given_name\n  description: Requests the user's given name claim.\n  standard: openid-connect-core\n- name: family_name\n  description: Requests the user's family name claim.\n  standard: openid-connect-core\n- name: nickname\n  description: Requests the user's nickname claim.\n  standard: openid-connect-core\n- name: picture\n  description: Requests the user's profile picture claim.\n  standard: openid-connect-core\n- name: created_at\n  description: Requests the account creation\
  \ timestamp claim (identity-provider extension).\n  standard: provider-extension\n- name: identities\n  description: Requests linked-identity metadata (identity-provider extension).\n  standard: provider-extension\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://authenticate.promptemr.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt/refs/heads/main/scopes/prompt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Electronic Medical Records
- Practice Management
- Physical Therapy
- Rehabilitation Therapy
- Health IT
- Medical Billing
- Patient Engagement
- Artificial Intelligence
token_urls: []
---
