---
authorization_urls:
- https://shopify.com/authentication/49573396633/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ecosoul Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EcoSoul Home publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EcoSoul Home API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/49573396633/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EcoSoul Home
provider_slug: ecosoul
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/49573396633/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/49573396633/oauth/token
  name: ShopifyCustomerAccountsOIDC
  source: https://www.ecosoulhome.com/.well-known/openid-configuration
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address (and email_verified claim).
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven access.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: ecosoul-scopes
source_filename: ecosoul-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ecosoulhome.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  source: https://www.ecosoulhome.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/49573396633/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/49573396633/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token identifying the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address (and email_verified claim).\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description:\
  \ Full access to the Customer Account MCP API surface for agent-driven access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecosoul/refs/heads/main/scopes/ecosoul-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Sustainability
- Home Goods
- Compostable
- Tableware
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/49573396633/oauth/token
---
