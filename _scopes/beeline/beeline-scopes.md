---
authorization_urls:
- https://shopify.com/authentication/18978919/oauth/authorize
description: ''
docs: https://beeline.co/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Beeline Scopes
name_suffix: OAuth Scopes
note: OAuth scopes advertised by the Shopify customer-account OIDC provider on the Beeline storefront. These are Shopify platform scopes for customer-account and UCP MCP access, not first-party Beeline product-API scopes.
overview: 'Beeline publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beeline API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/18978919/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beeline
provider_slug: beeline
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/18978919/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/18978919/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: https://beeline.co/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API (agent-facing customer-account operations).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: beeline-scopes
source_filename: beeline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://beeline.co/.well-known/openid-configuration\ndocs: https://beeline.co/.well-known/openid-configuration\nnote: >-\n  OAuth scopes advertised by the Shopify customer-account OIDC provider on the\n  Beeline storefront. These are Shopify platform scopes for customer-account and\n  UCP MCP access, not first-party Beeline product-API scopes.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: https://beeline.co/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/18978919/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/18978919/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n\
  \  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API (agent-facing customer-account operations).\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeline/refs/heads/main/scopes/beeline-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Navigation
- Cycling
- Motorcycle
- Hardware
- GPS
- Location
- Maps
- Mobile App
- Consumer Electronics
- Ecommerce
token_urls:
- https://shopify.com/authentication/18978919/oauth/token
---
