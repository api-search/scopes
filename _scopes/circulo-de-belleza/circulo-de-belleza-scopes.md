---
authorization_urls:
- https://shopify.com/authentication/25099010151/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Circulo De Belleza Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Circulo de Belleza publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Circulo de Belleza API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/25099010151/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Circulo de Belleza
provider_slug: circulo-de-belleza
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/25099010151/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/25099010151/oauth/token
  name: ShopifyCustomerAccountsOIDC
  source: well-known/circulo-de-belleza-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (issue an ID token for the customer)
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface (agent-driven customer account access)
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: circulo-de-belleza-scopes
source_filename: circulo-de-belleza-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.circulodebelleza.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  source: well-known/circulo-de-belleza-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/25099010151/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/25099010151/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (issue an ID token for the customer)\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and verification status\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account\
  \ MCP API surface (agent-driven customer account access)\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circulo-de-belleza/refs/heads/main/scopes/circulo-de-belleza-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beauty
- Cosmetics
- E-Commerce
- Retail
- Mexico
- Hair Care
- Professional Beauty Products
- Shopify
- Agent Commerce
token_urls:
- https://shopify.com/authentication/25099010151/oauth/token
---
