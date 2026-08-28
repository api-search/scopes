---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Numi Tea Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the scopes_supported array of the OAuth/OIDC discovery documents Numi Tea serves at numitea.com and account.numitea.com. Numi Tea publishes no scope reference page of its own -- these four are the complete advertised set.
overview: 'Numi Tea uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Numi Tea
provider_slug: numi-tea
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: numi-tea-scopes
source_filename: numi-tea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://numitea.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Read verbatim from the scopes_supported array of the OAuth/OIDC discovery\n  documents Numi Tea serves at numitea.com and account.numitea.com. Numi Tea\n  publishes no scope reference page of its own -- these four are the complete\n  advertised set.\nauthorization_server: https://shopify.com/authentication/82698961207\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OIDC scope; requests an id_token identifying the customer.\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: Standard OIDC scope; releases the email and email_verified claims.\n    standard: OpenID Connect Core 1.0\n  - name: 'customer-account-api:full'\n    description: >-\n      Full access to the Shopify Customer Account API for the authenticated\n      customer -- orders, addresses, profile and subscription\
  \ state on this store.\n    vendor: shopify\n  - name: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the customer-account MCP API. This is the scope that lets an\n      agent act on the authenticated customer's account through MCP rather than\n      through the storefront UI.\n    vendor: shopify\ngranularity: coarse\ngranularity_note: >-\n  Both non-standard scopes are \":full\". There is no read-only or per-resource\n  split, so an agent granted customer-account access to place an order also holds\n  the ability to read the customer's full order history and profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numi-tea/refs/heads/main/scopes/numi-tea-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Tea
- Beverages
- Consumer Packaged Goods
- Retail
- E-Commerce
- Organic
- Fair Trade
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
token_urls: []
---
