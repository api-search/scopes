---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Parsley Health Scopes
name_suffix: OAuth Scopes
note: These are the OAuth 2.0 / OIDC scopes advertised by the authorization server discovered on Parsley Health's store hostname. They govern customer accounts for the Parsley Health supplement store only. The authorization server is Shopify's per-shop issuer (shop 24996151350) — Parsley Health publishes no scope reference of its own, and there are no clinical, member or medical-record scopes anywhere on its public surface. Descriptions below are the platform's documented meaning; only the scope STRINGS are verbatim from the discovery document.
overview: 'Parsley Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parsley Health
provider_slug: parsley-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: parsley-health-scopes
source_filename: parsley-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  https://store.parsleyhealth.com/.well-known/openid-configuration and\n  https://store.parsleyhealth.com/.well-known/oauth-authorization-server\n  (both HTTP 200, scopes_supported read verbatim, 2026-08-15)\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  These are the OAuth 2.0 / OIDC scopes advertised by the authorization server discovered\n  on Parsley Health's store hostname. They govern customer accounts for the Parsley\n  Health supplement store only. The authorization server is Shopify's per-shop issuer\n  (shop 24996151350) — Parsley Health publishes no scope reference of its own, and there\n  are no clinical, member or medical-record scopes anywhere on its public surface.\n  Descriptions below are the platform's documented meaning; only the scope STRINGS are\n  verbatim from the discovery document.\nauthorization_server: https://shopify.com/authentication/24996151350\nscope_count: 4\nscopes:\n- name: openid\n\
  \  description: Standard OIDC scope — request an ID token for the authenticated store customer.\n  standard: true\n- name: email\n  description: Standard OIDC scope — release the customer's email address and email_verified claim.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the store's Customer Account API on behalf of the signed-in customer (orders, addresses, profile).\n  standard: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API on behalf of the signed-in customer — the\n    authenticated counterpart to the anonymous UCP/MCP commerce endpoint.\n  standard: false\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\nnot_found:\n- surface: clinical / member API\n  note: No OAuth scopes of any kind are published for the Parsley Health medical practice or member application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsley-health/refs/heads/main/scopes/parsley-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Healthcare
- Telehealth
- Telemedicine
- Functional Medicine
- Primary Care
- Wellness
- Nutrition
- Diagnostics
- Lab Testing
- Membership
- Digital Health
- Consumer Health
- Ecommerce
- Agentic Commerce
- MCP
- Supplements
token_urls: []
---
