---
authorization_urls: []
description: ''
docs: https://www.drinkhint.com/.well-known/openid-configuration
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: probed
name: Hint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hint publishes 4 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hint API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hint
provider_slug: hint
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the buyer.
  flows: []
  scope: openid
- description: Releases the buyer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer (orders, addresses, subscriptions, profile). Observed as the scope requested by the storefront login flow.
  flows: []
  scope: customer-account-api:full
- description: Full access to the authenticated Customer Account MCP API for the signed-in buyer — the logged-in counterpart to the anonymous storefront commerce MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: hint-scopes
source_filename: hint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://www.drinkhint.com/.well-known/openid-configuration (scopes_supported), HTTP 200\ndocs: https://www.drinkhint.com/.well-known/openid-configuration\nsummary: >-\n  The only scope surface Hint's hosts publish is the Shopify Customer Accounts OpenID Connect\n  discovery document. Four scopes are advertised. The agentic commerce MCP endpoint itself is\n  anonymous and declares no scopes.\nauthorization_server: https://shopify.com/authentication/1430159418\nflows:\n- type: authorization_code\n  pkce: S256\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token for the buyer.\n- name: email\n  description: Releases the buyer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in buyer (orders, addresses,\n    subscriptions, profile). Observed as the scope requested\
  \ by the storefront login flow.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the authenticated Customer Account MCP API for the signed-in buyer — the\n    logged-in counterpart to the anonymous storefront commerce MCP endpoint.\nnotes:\n- Hint publishes no scope reference page of its own; these values are read directly from the\n  machine-readable discovery document served on its host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint/refs/heads/main/scopes/hint-scopes.yml
summary_line: 4 scopes · authorization_code
tags:
- Company
- Beverages
- Consumer Packaged Goods
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
token_bound: false
token_urls: []
---
