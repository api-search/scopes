---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pantheryx Scopes
name_suffix: OAuth Scopes
note: These are Shopify customer-account scopes exposed by the identity provider behind the two PanTheryx brand storefronts. PanTheryx publishes no scope reference of its own, and there is no provider-authored docs page to enrich these descriptions from — the descriptions below are read from the scope names and the Shopify authorization-server metadata only.
overview: 'PanTheryx uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PanTheryx
provider_slug: pantheryx
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: pantheryx-scopes
source_filename: pantheryx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from https://relesium.com/.well-known/oauth-authorization-server\n  and https://www.lifesfirstnaturals.com/.well-known/oauth-authorization-server (both HTTP 200,\n  fetched anonymously 2026-08-26).\nnote: >-\n  These are Shopify customer-account scopes exposed by the identity provider behind the two\n  PanTheryx brand storefronts. PanTheryx publishes no scope reference of its own, and there is no\n  provider-authored docs page to enrich these descriptions from — the descriptions below are read\n  from the scope names and the Shopify authorization-server metadata only.\nauthorization_servers:\n- host: relesium.com\n  issuer: https://shopify.com/authentication/60191506528\n- host: www.lifesfirstnaturals.com\n  issuer: https://shopify.com/authentication/27073282091\ncode_challenge_methods_supported:\n- S256\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID\
  \ token for the signed-in customer.\n- name: email\n  description: Releases the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API — the authenticated counterpart to the anonymous\n    UCP shopping MCP endpoint, scoped to one signed-in customer's account.\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantheryx/refs/heads/main/scopes/pantheryx-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Nutrition
- Biotechnology
- Life Sciences
- Consumer Health
- Dietary Supplements
- Colostrum
- Animal Health
- Ecommerce
- Agentic Commerce
token_urls: []
---
