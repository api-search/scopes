---
authorization_urls:
- https://shopify.com/authentication/5451009/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: True Botanicals Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'True Botanicals publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the True Botanicals API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/5451009/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: True Botanicals
provider_slug: true-botanicals
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope — requests an ID token identifying the signed-in customer.
  flows: []
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer — profile, addresses, orders and subscriptions for this shop.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer — the authenticated counterpart to the anonymous UCP shopping MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: true-botanicals-scopes
source_filename: true-botanicals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://truebotanicals.com/.well-known/openid-configuration (scopes_supported, HTTP 200, 2026-08-30)\ndocs: https://shopify.dev/docs/api/customer\nissuer: https://shopify.com/authentication/5451009\nflows:\n- type: authorizationCode\n  authorizationUrl: https://shopify.com/authentication/5451009/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/5451009/oauth/token\n  pkce: S256\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope — requests an ID token identifying the signed-in customer.\n  standard: OIDC Core 1.0\n- name: email\n  description: Releases the customer's email and email_verified claims.\n  standard: OIDC Core 1.0\n- name: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer — profile,\n    addresses, orders and subscriptions for this shop.\n  standard: Shopify\n- name: 'customer-account-mcp-api:full'\n  description:\
  \ Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer — the\n    authenticated counterpart to the anonymous UCP shopping MCP endpoint.\n  standard: Shopify\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\nnotes:\n- 'These are the only scopes this issuer advertises. There is no granular read/write split — customer-account\n  access is all-or-nothing at :full.'\n- 'The scopes govern customer-account access, not merchant/admin access. Nothing here grants an agent\n  privileged access to True Botanicals'' own store data.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-botanicals/refs/heads/main/scopes/true-botanicals-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Beauty
- Skincare
- Consumer Goods
- Direct to Consumer
- Agentic Commerce
- Shopify
- MCP
- Universal Commerce Protocol
token_bound: false
token_urls:
- https://shopify.com/authentication/5451009/oauth/token
---
