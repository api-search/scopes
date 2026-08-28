---
authorization_urls:
- https://shopify.com/authentication/64317849670/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Malk Organics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MALK Organics publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MALK Organics API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/64317849670/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MALK Organics
provider_slug: malk-organics
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/64317849670/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/64317849670/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/malk-organics-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the buyer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven commerce on behalf of the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: malk-organics-scopes
source_filename: malk-organics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://malkorganics.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth 2.0 / OIDC scopes advertised in scopes_supported by MALK Organics's Shopify Customer\n  Accounts authorization server, read from the discovery document served on malkorganics.com.\n  Descriptions reflect the Shopify Customer Account API and its MCP surface. MALK publishes no\n  OpenAPI, so there is no securitySchemes block to derive from.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/malk-organics-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/64317849670/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/64317849670/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the buyer.\n  flows: [authorizationCode]\n  sources: [well-known/malk-organics-openid-configuration.json]\n\
  - scope: email\n  description: Access the buyer's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/malk-organics-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.\n  flows: [authorizationCode]\n  sources: [well-known/malk-organics-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API surface for agent-driven commerce on behalf of\n    the signed-in buyer.\n  flows: [authorizationCode]\n  sources: [well-known/malk-organics-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/malk-organics/refs/heads/main/scopes/malk-organics-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Food and Beverage
- Consumer Packaged Goods
- Plant-Based
- Organic
- Direct to Consumer
- Agent Commerce
- MCP
- Shopify
token_urls:
- https://shopify.com/authentication/64317849670/oauth/token
---
