---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clarify Health Scopes
name_suffix: OAuth Scopes
note: Clarify Health publishes no scope or permission reference page — there is no developer portal to publish one on. These are the scopes the two live OIDC issuers advertise in their own discovery documents. They are ALL standard OpenID Connect / OAuth 2.0 identity scopes; not one Clarify-specific resource scope is advertised anywhere, which is the finding. A custom Okta authorization server may carry product scopes, but /oauth2/default/.well-known/openid-configuration returns 401 (E0000015) so they are not anonymously discoverable.
overview: 'Clarify Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clarify Health
provider_slug: clarify-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: clarify-health-scopes
source_filename: clarify-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from\n  https://auth.clarifyhealth.com/.well-known/openid-configuration (200) and\n  https://okta.clarifyhealth.com/.well-known/openid-configuration (200), fetched 2026-08-15\ndocs: null\nnote: >-\n  Clarify Health publishes no scope or permission reference page — there is no developer\n  portal to publish one on. These are the scopes the two live OIDC issuers advertise in\n  their own discovery documents. They are ALL standard OpenID Connect / OAuth 2.0 identity\n  scopes; not one Clarify-specific resource scope is advertised anywhere, which is the\n  finding. A custom Okta authorization server may carry product scopes, but\n  /oauth2/default/.well-known/openid-configuration returns 401 (E0000015) so they are not\n  anonymously discoverable.\nissuers:\n- issuer: https://auth.clarifyhealth.com/\n  platform: Auth0\n  scope_count: 14\n  scopes:\n  - name: openid\n    description: Request an\
  \ ID token (OpenID Connect core).\n    standard: true\n  - name: profile\n    description: Basic profile claims for the authenticated user.\n    standard: true\n  - name: offline_access\n    description: Issue a refresh token.\n    standard: true\n  - name: name\n    description: Full name claim.\n    standard: true\n  - name: given_name\n    description: Given name claim.\n    standard: true\n  - name: family_name\n    description: Family name claim.\n    standard: true\n  - name: nickname\n    description: Nickname claim.\n    standard: true\n  - name: email\n    description: Email address claim.\n    standard: true\n  - name: email_verified\n    description: Email verification status claim.\n    standard: true\n  - name: picture\n    description: Profile picture claim.\n    standard: true\n  - name: created_at\n    description: Account creation timestamp claim (Auth0 extension).\n    standard: false\n  - name: identities\n    description: Linked identity provider records (Auth0 extension).\n\
  \    standard: false\n  - name: phone\n    description: Phone number claim.\n    standard: true\n  - name: address\n    description: Address claim.\n    standard: true\n- issuer: https://okta.clarifyhealth.com\n  platform: Okta\n  scope_count: 7\n  scopes:\n  - name: openid\n    description: Request an ID token (OpenID Connect core).\n    standard: true\n  - name: email\n    description: Email address claim.\n    standard: true\n  - name: profile\n    description: Basic profile claims.\n    standard: true\n  - name: address\n    description: Address claim.\n    standard: true\n  - name: phone\n    description: Phone number claim.\n    standard: true\n  - name: offline_access\n    description: Issue a refresh token.\n    standard: true\n  - name: groups\n    description: Group memberships of the authenticated user (Okta org server).\n    standard: false\nsummary:\n  total_scopes: 21\n  resource_scopes: 0\n  identity_scopes: 21\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarify-health/refs/heads/main/scopes/clarify-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health Tech
- Healthcare Analytics
- Health Data
- Outcomes
- Referral Intelligence
- Payers
- Life Sciences
token_urls: []
---
