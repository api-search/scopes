---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the IM8 Health Shopify Customer Account authorization server (scopes_supported in the store's OIDC discovery document). These are Shopify platform Customer Account scopes exposed under the im8health.com account host.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Im8 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IM8 Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IM8 Health
provider_slug: im8
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: im8-scopes
source_filename: im8-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://im8health.com/.well-known/openid-configuration\ntype: OAuthScopes\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the IM8 Health Shopify Customer\n  Account authorization server (scopes_supported in the store's OIDC discovery\n  document). These are Shopify platform Customer Account scopes exposed under the\n  im8health.com account host.\nauthorization_server: https://shopify.com/authentication/63744606375\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; issue an ID token identifying the buyer.\n- name: email\n  description: Access the buyer's email address and verification status.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API — authorizes MCP-driven agents to\n    act on the buyer's account (orders,\
  \ profile) under the Customer Account API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/im8/refs/heads/main/scopes/im8-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Wellness
- Supplements
- Nutrition
- Ecommerce
- Direct-to-Consumer
- Agentic Commerce
- Shopify
- UCP
- MCP
token_urls: []
---
