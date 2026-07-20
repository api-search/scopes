---
authorization_urls:
- https://account.barnandwillow.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Barn And Willow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Barn & Willow publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Barn & Willow API on a user''s behalf.


  Tokens are issued from https://account.barnandwillow.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Barn & Willow
provider_slug: barn-and-willow
schemes:
- flows:
  - authorizationUrl: https://account.barnandwillow.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.barnandwillow.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/barn-and-willow-openid-configuration.json
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
- description: Access the authenticated customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agentic (MCP) commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: barn-and-willow-scopes
source_filename: barn-and-willow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://barnandwillow.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth scopes advertised by the Shopify Customer Account API OIDC discovery\n  document for barnandwillow.com (scopes_supported).\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/barn-and-willow-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.barnandwillow.com/authentication/oauth/authorize\n    tokenUrl: https://account.barnandwillow.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/barn-and-willow-openid-configuration.json]\n- scope: email\n  description: Access the authenticated customer's email address and verification status.\n  flows: [authorizationCode]\n  sources: [well-known/barn-and-willow-openid-configuration.json]\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/barn-and-willow-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agentic (MCP) commerce.\n  flows: [authorizationCode]\n  sources: [well-known/barn-and-willow-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barn-and-willow/refs/heads/main/scopes/barn-and-willow-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-commerce
- Retail
- Home Furnishings
- Window Treatments
- Agentic Commerce
- Shopify
- Direct to Consumer
token_urls:
- https://account.barnandwillow.com/authentication/oauth/token
---
