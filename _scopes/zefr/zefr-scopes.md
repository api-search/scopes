---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zefr Scopes
name_suffix: OAuth Scopes
note: These are the scopes Zefr's own identity provider (Auth0 custom domain login.zefr.com) advertises in its OpenID Connect discovery document, read verbatim. They are the standard OIDC identity-layer scopes — Zefr publishes NO product/API scope reference, and no audience-scoped permissions for any Zefr API. Recorded because they are genuinely published and machine-readable, not because they describe a product authorization model.
overview: 'Zefr uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zefr
provider_slug: zefr
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zefr-scopes
source_filename: zefr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://login.zefr.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes Zefr's own identity provider (Auth0 custom domain login.zefr.com)\n  advertises in its OpenID Connect discovery document, read verbatim. They are the standard\n  OIDC identity-layer scopes — Zefr publishes NO product/API scope reference, and no\n  audience-scoped permissions for any Zefr API. Recorded because they are genuinely published\n  and machine-readable, not because they describe a product authorization model.\nissuer: https://login.zefr.com/\ndocs: null\ndocs_note: No scopes or permissions reference page is published anywhere on zefr.com.\nscope_count: 14\nscopes:\n- name: openid\n  description: Required for OpenID Connect; returns an ID token.\n  layer: identity\n- name: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture, created_at).\n  layer: identity\n- name: offline_access\n  description:\
  \ Issues a refresh token for long-lived access.\n  layer: identity\n- name: name\n  description: The end user's full name claim.\n  layer: identity\n- name: given_name\n  description: The end user's given name claim.\n  layer: identity\n- name: family_name\n  description: The end user's family name claim.\n  layer: identity\n- name: nickname\n  description: The end user's nickname claim.\n  layer: identity\n- name: email\n  description: The end user's email address claim.\n  layer: identity\n- name: email_verified\n  description: Whether the end user's email address has been verified.\n  layer: identity\n- name: picture\n  description: URL of the end user's profile picture.\n  layer: identity\n- name: created_at\n  description: Account creation timestamp claim.\n  layer: identity\n- name: identities\n  description: Linked identity-provider connections for the account (Auth0 extension).\n  layer: identity\n- name: phone\n  description: The end user's phone number claim.\n  layer: identity\n\
  - name: address\n  description: The end user's address claim.\n  layer: identity\nproduct_scopes:\n  published: false\n  note: >-\n    No Zefr product API scopes (brand suitability, measurement, reporting, classification)\n    are published. A machine-to-machine client would need an audience and scopes issued\n    privately by Zefr; neither is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zefr/refs/heads/main/scopes/zefr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AdTech
- Brand Safety
- Brand Suitability
- Content Intelligence
- Content Moderation
- Video
- Social-Media
- Advertising
- Media Measurement
- Machine-Learning
token_urls: []
---
