---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Urbanstems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UrbanStems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UrbanStems
provider_slug: urbanstems
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: urbanstems-scopes
source_filename: urbanstems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://urbanstems.com/.well-known/openid-configuration (HTTP 200, scopes_supported)\nname: UrbanStems OAuth scopes\nslug: urbanstems\ndocs: null\ndocs_note: >-\n  UrbanStems publishes no scopes/permissions reference page of its own. The scope list below is read\n  verbatim from the machine-readable OIDC discovery document served at the UrbanStems host; the\n  descriptions are the standard meanings of those identifiers, not UrbanStems prose.\n\nauthorization_server:\n  issuer: https://shopify.com/authentication/69340168440\n  discovery: https://urbanstems.com/.well-known/openid-configuration\n  authorization_endpoint: https://tracking.urbanstems.com/authentication/oauth/authorize\n  token_endpoint: https://tracking.urbanstems.com/authentication/oauth/token\n\nscope_count: 4\nscopes:\n- name: openid\n  standard: OpenID Connect Core\n  description: Request an ID token identifying the signed-in customer.\n- name: email\n  standard:\
  \ OpenID Connect Core\n  description: Release the email and email_verified claims for the signed-in customer.\n- name: customer-account-api:full\n  standard: Shopify Customer Account API\n  description: >-\n    Full access to the customer account surface on behalf of the signed-in customer — orders,\n    addresses, profile and subscription state for this shop.\n- name: customer-account-mcp-api:full\n  standard: Shopify Customer Account MCP API\n  description: >-\n    Full access to the customer-account MCP surface on behalf of the signed-in customer. This is the\n    authenticated companion to the anonymous commerce MCP endpoint; it is the scope an agent would\n    hold to act on a specific buyer's account rather than on the public catalog.\n\nnot_scoped:\n  surface: UrbanStems Commerce MCP API (https://274513-24.myshopify.com/api/ucp/mcp)\n  note: >-\n    The UCP commerce endpoint is anonymous — it accepts no bearer token and therefore has no scope\n    model. Buyer authority is carried\
  \ per-call by the payment instrument, not by an OAuth grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanstems/refs/heads/main/scopes/urbanstems-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Flowers
- Gifting
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
token_urls: []
---
