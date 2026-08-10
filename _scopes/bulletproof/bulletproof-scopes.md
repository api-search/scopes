---
authorization_urls:
- https://account.bulletproof.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bulletproof Scopes
name_suffix: OAuth Scopes
note: Scopes come from the live OAuth 2.0 / OpenID Connect discovery documents served on the Bulletproof hosts (identical payload at shop., account. and the myshopify origin). Bulletproof publishes no scope reference page of its own — these four are the complete scopes_supported list as advertised, nothing has been added.
overview: 'BulletProof publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BulletProof API on a user''s behalf.


  Tokens are issued from https://account.bulletproof.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BulletProof
provider_slug: bulletproof
schemes:
- flows:
  - authorizationUrl: https://account.bulletproof.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.bulletproof.com/authentication/oauth/token
  name: customer-accounts
  source: https://shop.bulletproof.com/.well-known/openid-configuration
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for the signed-in customer — profile, addresses, orders and subscriptions.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer account MCP API — the agent-facing projection of the same customer account data. Notable as an explicitly agent-scoped grant.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bulletproof-scopes
source_filename: bulletproof-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://shop.bulletproof.com/.well-known/openid-configuration\nnote: >-\n  Scopes come from the live OAuth 2.0 / OpenID Connect discovery documents served on\n  the Bulletproof hosts (identical payload at shop., account. and the myshopify origin).\n  Bulletproof publishes no scope reference page of its own — these four are the complete\n  scopes_supported list as advertised, nothing has been added.\nissuer: https://shopify.com/authentication/434700319\nschemes:\n- name: customer-accounts\n  type: openIdConnect\n  source: https://shop.bulletproof.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.bulletproof.com/authentication/oauth/authorize\n    tokenUrl: https://account.bulletproof.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.\n  flows: [authorizationCode]\n\
  \  sources: ['well-known/bulletproof-openid-configuration.json']\n- scope: email\n  description: Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: ['well-known/bulletproof-openid-configuration.json']\n- scope: customer-account-api:full\n  description: >-\n    Full access to the customer account API for the signed-in customer — profile,\n    addresses, orders and subscriptions.\n  flows: [authorizationCode]\n  sources: ['well-known/bulletproof-openid-configuration.json']\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer account MCP API — the agent-facing projection of the\n    same customer account data. Notable as an explicitly agent-scoped grant.\n  flows: [authorizationCode]\n  sources: ['well-known/bulletproof-openid-configuration.json']\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ngaps:\n- >-\n  The UCP MCP endpoint at /api/ucp/mcp requires a JWT for\
  \ order and checkout tools but\n  does not advertise which of these scopes mints it; the error body points at\n  shopify.dev rather than a Bulletproof-owned page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulletproof/refs/heads/main/scopes/bulletproof-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Health and Wellness
- Supplements
- Ecommerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
token_urls:
- https://account.bulletproof.com/authentication/oauth/token
---
