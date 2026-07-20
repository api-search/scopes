---
authorization_urls:
- https://shopify.com/authentication/70535250059/oauth/authorize
description: ''
docs: https://italist.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Italist Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Shopify Customer Account authorization server serving italist.com. These govern the buyer's customer-account session, including the customer-account MCP surface.
overview: 'Italist publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Italist API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/70535250059/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Italist
provider_slug: italist
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/70535250059/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/70535250059/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: https://italist.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: italist-scopes
source_filename: italist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://italist.com/.well-known/openid-configuration\ndocs: https://italist.com/.well-known/openid-configuration\nnote: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account authorization server\n  serving italist.com. These govern the buyer's customer-account session, including\n  the customer-account MCP surface.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: https://italist.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/70535250059/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/70535250059/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address and verification status.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description:\
  \ Full access to the Shopify Customer Account API for the signed-in buyer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for the signed-in buyer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/italist/refs/heads/main/scopes/italist-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-commerce
- Retail
- Fashion
- Luxury
- Marketplace
- Shopify
- Agentic Commerce
- MCP
token_urls:
- https://shopify.com/authentication/70535250059/oauth/token
---
