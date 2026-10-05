---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mori Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 / OIDC scopes advertised by the Shopify Customer Account API discovery document for this store. customer-account-mcp-api:full authorizes the authenticated Customer Account MCP surface; the anonymous storefront MCP at /api/mcp requires no scope.
overview: 'MORI publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MORI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MORI
provider_slug: mori
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; returns an ID token identifying the signed-in customer.
  flows: []
  scope: openid
- description: Grants access to the customer's email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).
  flows: []
  scope: customer-account-api:full
- description: Full access to the authenticated Customer Account MCP API surface for the signed-in customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: mori-scopes
source_filename: mori-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: scopes_supported in live https://babymori.com/.well-known/openid-configuration (Shopify Customer Account API)\nissuer: https://shopify.com/authentication/6726617\nnote: >-\n  OAuth 2.0 / OIDC scopes advertised by the Shopify Customer Account API\n  discovery document for this store. customer-account-mcp-api:full authorizes\n  the authenticated Customer Account MCP surface; the anonymous storefront MCP\n  at /api/mcp requires no scope.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; returns an ID token identifying the signed-in customer.\n- name: email\n  description: Grants access to the customer's email and email_verified claims.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).\n- name: customer-account-mcp-api:full\n  description: Full access to the authenticated Customer Account MCP API surface\
  \ for the signed-in customer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mori/refs/heads/main/scopes/mori-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Retail
- E-Commerce
- Baby Products
- Consumer Goods
- Apparel
- Direct to Consumer
- Shopify
- MCP
- Agent-Native
- Universal Commerce Protocol
token_bound: false
token_urls: []
---
