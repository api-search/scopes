---
authorization_urls:
- https://shopify.com/authentication/76759498890/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kimba Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kimba publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kimba API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/76759498890/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kimba
provider_slug: kimba
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/76759498890/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/76759498890/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/kimba-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (subject identifier).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven customer operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: kimba-scopes
source_filename: kimba-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://kimba.ai/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth scopes advertised by the Shopify Customer Account API OIDC provider backing\n  the Kimba storefront (scopes_supported in the published openid-configuration).\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/kimba-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/76759498890/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/76759498890/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (subject identifier).\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n  flows: [authorizationCode]\n\
  - scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API for agent-driven customer operations.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimba/refs/heads/main/scopes/kimba-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Sleep Technology
- Consumer Hardware
- Health & Wellness
- Artificial Intelligence
- Wearables
- E-Commerce
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/76759498890/oauth/token
---
