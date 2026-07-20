---
authorization_urls:
- https://shopify.com/authentication/89171296584/oauth/authorize
description: ''
docs: https://footway.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Footway Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Footway publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Footway API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/89171296584/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Footway
provider_slug: footway
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/89171296584/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/89171296584/oauth/token
  issuer: https://shopify.com/authentication/89171296584
  name: ShopifyCustomerAccount
  source: well-known/footway-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API, enabling agent-driven account operations for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: footway-scopes
source_filename: footway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://footway.com/.well-known/openid-configuration\ndocs: https://footway.com/.well-known/oauth-authorization-server\nschemes:\n- name: ShopifyCustomerAccount\n  source: well-known/footway-openid-configuration.json\n  issuer: https://shopify.com/authentication/89171296584\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/89171296584/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/89171296584/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/footway-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/footway-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the\
  \ Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/footway-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API, enabling agent-driven account operations for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/footway-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footway/refs/heads/main/scopes/footway-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- E-commerce
- Marketplace
- Retail
- Footwear
- Fashion
- Shopify
- Agent Commerce
- UCP
- MCP
- Nordic
token_urls:
- https://shopify.com/authentication/89171296584/oauth/token
---
