---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Maisonette Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py was not usable here — it reads OpenAPI oauth2 securitySchemes and Maisonette publishes no OpenAPI. These scopes are read verbatim from the store's own machine-readable authorization-server metadata. The authorization server is Shopify's hosted customer-account issuer for Maisonette's shop (id 58323238975), which is why the scope names carry Shopify's customer-account naming.
overview: 'Maisonette uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Maisonette
provider_slug: maisonette
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: maisonette-scopes
source_filename: maisonette-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://www.maisonette.com/.well-known/openid-configuration (and the identical\n  /.well-known/oauth-authorization-server), fetched 2026-08-25, HTTP 200.\nnote: 'derive-oauth-scopes.py was not usable here — it reads OpenAPI oauth2 securitySchemes\n  and Maisonette publishes no OpenAPI. These scopes are read verbatim from the store''s\n  own machine-readable authorization-server metadata. The authorization server is Shopify''s\n  hosted customer-account issuer for Maisonette''s shop (id 58323238975), which is\n  why the scope names carry Shopify''s customer-account naming.'\nissuer: https://shopify.com/authentication/58323238975\nauthorization_endpoint: https://shopify.com/authentication/58323238975/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/58323238975/oauth/token\ngrant_types:\n- authorization_code\n- refresh_token\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\npkce_methods:\n- S256\nscope_count:\
  \ 4\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated Maisonette\n    customer.\n- name: email\n  description: Releases the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the authenticated buyer's Maisonette customer account\n    — profile, addresses, and order history — through Shopify's Customer Account API.\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account surface through MCP, i.e. lets an\n    agent act on the signed-in buyer's account rather than only on anonymous catalog\n    and cart state.\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\ndocs: null\ndocs_note: Maisonette publishes no scopes/permissions reference page of its own. The\n  scope semantics above are described from Shopify's customer-account model; the scope\n  strings themselves are verbatim from Maisonette's\
  \ own discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maisonette/refs/heads/main/scopes/maisonette-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Retail
- E-Commerce
- Marketplace
- Shopping
- Children
- Baby
- Apparel
- Home
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
token_urls: []
---
