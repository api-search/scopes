---
authorization_urls:
- https://shopify.com/authentication/5260181607/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: The Beard Club Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Beard Club publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Beard Club API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/5260181607/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Beard Club
provider_slug: the-beard-club
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/5260181607/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/5260181607/oauth/token
  issuer: https://shopify.com/authentication/5260181607
  name: ShopifyCustomerAccount
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token for the customer.
  flows: []
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the agent-facing customer surface.
  flows: []
  scope: customer-account-mcp-api:full
slug: the-beard-club-scopes
source_filename: the-beard-club-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thebeardclub.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccount\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/5260181607\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/5260181607/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/5260181607/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token for the customer.\n  sources:\n  - well-known/the-beard-club-openid-configuration.json\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  sources:\n  - well-known/the-beard-club-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  sources:\n  - well-known/the-beard-club-openid-configuration.json\n\
  - scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API — the agent-facing customer surface.\n  sources:\n  - well-known/the-beard-club-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-beard-club/refs/heads/main/scopes/the-beard-club-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-commerce
- Retail
- Men's Grooming
- Consumer Goods
- Shopify
- Agent Commerce
- UCP
- MCP
- Subscription
token_urls:
- https://shopify.com/authentication/5260181607/oauth/token
---
