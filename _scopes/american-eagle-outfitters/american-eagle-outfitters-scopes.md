---
authorization_urls: []
description: ''
docs: https://www.unsubscribed.com/agents.md
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: American Eagle Outfitters Scopes
name_suffix: OAuth Scopes
note: These are the OpenID Connect scopes Shopify advertises for customer accounts on the AEO brand storefront www.unsubscribed.com. American Eagle Outfitters publishes no OAuth scope reference of its own — there is no developer programme on www.ae.com to have one. The scopes are read verbatim from scopes_supported in the live discovery document; no descriptions are published by the provider, so the descriptions below are stated as derived readings of the scope names and are marked as such.
overview: 'American Eagle Outfitters publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the American Eagle Outfitters API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: American Eagle Outfitters
provider_slug: american-eagle-outfitters
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the shopper.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; releases the shopper's email address claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in shopper (orders, addresses, profile).
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in shopper — the authenticated counterpart to the anonymous UCP shopping endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: american-eagle-outfitters-scopes
source_filename: american-eagle-outfitters-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://www.unsubscribed.com/.well-known/openid-configuration\ndocs: https://www.unsubscribed.com/agents.md\nnote: >-\n  These are the OpenID Connect scopes Shopify advertises for customer accounts on the AEO\n  brand storefront www.unsubscribed.com. American Eagle Outfitters publishes no OAuth scope\n  reference of its own — there is no developer programme on www.ae.com to have one. The\n  scopes are read verbatim from scopes_supported in the live discovery document; no\n  descriptions are published by the provider, so the descriptions below are stated as\n  derived readings of the scope names and are marked as such.\nauthorization_server: https://shopify.com/authentication/55041261720\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the shopper.\n  description_method: derived\n- name: email\n  description: Standard OpenID Connect scope; releases the shopper's\
  \ email address claim.\n  description_method: derived\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in shopper (orders, addresses, profile).\n  description_method: derived\n- name: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in shopper — the authenticated counterpart to the anonymous UCP shopping endpoint.\n  description_method: derived\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-eagle-outfitters/refs/heads/main/scopes/american-eagle-outfitters-scopes.yml
summary_line: 4 scopes
tags:
- Retail
- E-Commerce
- Fashion
- Apparel
- Consumer Goods
- Fortune 1000
token_bound: false
token_urls: []
---
