---
authorization_urls:
- https://account.therabody.com/authentication/oauth/authorize
description: ''
docs: https://account.therabody.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Therabody Scopes
name_suffix: OAuth Scopes
note: Scopes are published by the customer-account authorization server discovery document, not by an OpenAPI securityScheme — Therabody publishes no OpenAPI. The UCP commerce MCP server is not scope-gated; it gates checkout completion on explicit buyer approval instead.
overview: 'Therabody publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Therabody API on a user''s behalf.


  Tokens are issued from https://account.therabody.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Therabody
provider_slug: therabody
schemes:
- flows:
  - authorizationUrl: https://account.therabody.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.therabody.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/67140976867
  name: ShopifyCustomerAccountOIDC
  source: well-known/therabody-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer (orders, addresses, payment methods, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP tool surface for the authenticated customer (order status, store credit balances, return requests).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: therabody-scopes
source_filename: therabody-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://www.therabody.com/.well-known/openid-configuration\ndocs: https://account.therabody.com/.well-known/oauth-authorization-server\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  issuer: https://shopify.com/authentication/67140976867\n  source: well-known/therabody-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.therabody.com/authentication/oauth/authorize\n    tokenUrl: https://account.therabody.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/therabody-openid-configuration.json\n- scope: email\n  description: Access to the customer email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/therabody-openid-configuration.json\n- scope: customer-account-api:full\n\
  \  description: Full access to the Shopify Customer Account API for the authenticated customer (orders,\n    addresses, payment methods, profile).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/therabody-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP tool surface for the authenticated customer (order\n    status, store credit balances, return requests).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/therabody-openid-configuration.json\nnote: Scopes are published by the customer-account authorization server discovery document, not by an\n  OpenAPI securityScheme — Therabody publishes no OpenAPI. The UCP commerce MCP server is not scope-gated;\n  it gates checkout completion on explicit buyer approval instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/therabody/refs/heads/main/scopes/therabody-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Wellness
- Health
- Consumer Products
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- Model Context Protocol
- GraphQL
- Universal Commerce Protocol
token_urls:
- https://account.therabody.com/authentication/oauth/token
---
