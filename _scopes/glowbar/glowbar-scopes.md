---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Glowbar Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from the `scopes_supported` array of the OIDC discovery document served by glowbar.com for Shopify Customer Accounts shop 44884033689. Glowbar publishes no scope reference page of its own; descriptions below state what each scope grants according to the discovery document and the observed protected resource, and are marked as such rather than quoted from a Glowbar doc.
overview: 'Glowbar uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Glowbar
provider_slug: glowbar
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: glowbar-scopes
source_filename: glowbar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://glowbar.com/.well-known/openid-configuration\nnote: >-\n  Scopes read verbatim from the `scopes_supported` array of the OIDC discovery document served\n  by glowbar.com for Shopify Customer Accounts shop 44884033689. Glowbar publishes no scope\n  reference page of its own; descriptions below state what each scope grants according to the\n  discovery document and the observed protected resource, and are marked as such rather than\n  quoted from a Glowbar doc.\nauthorization_server: https://shopify.com/authentication/44884033689\nprotected_resource: https://glowbar.com\nflows:\n- type: authorization_code\n  pkce: S256\n  authorization_url: https://shopify.com/authentication/44884033689/oauth/authorize\n  token_url: https://shopify.com/authentication/44884033689/oauth/token\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the signed-in buyer.\n  source: scopes_supported\n\
  - name: email\n  description: Releases the buyer's email address and email_verified claim.\n  source: scopes_supported\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer — profile, addresses, and order history on the Glowbar store.\n  source: scopes_supported\n- name: customer-account-mcp-api:full\n  description: Full access to the buyer-scoped Customer Account MCP API, the authenticated counterpart to the anonymous storefront UCP/MCP endpoint.\n  source: scopes_supported\nscope_count: 4\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ndocs: null\ndocs_note: No Glowbar-published scopes or permissions reference page exists; the discovery document is the only machine-readable source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glowbar/refs/heads/main/scopes/glowbar-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Skincare
- Beauty
- Retail
- Commerce
- Ecommerce
- Consumer Services
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Memberships
token_urls: []
---
