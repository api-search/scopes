---
authorization_urls:
- https://account.cuyana.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cuyana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cuyana publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cuyana API on a user''s behalf.


  Tokens are issued from https://account.cuyana.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cuyana
provider_slug: cuyana
schemes:
- flows:
  - authorizationUrl: https://account.cuyana.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.cuyana.com/authentication/oauth/token
  name: ShopifyCustomerAccountOAuth
  source: well-known/cuyana-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (issue an ID token).
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: cuyana-scopes
source_filename: cuyana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cuyana.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  scopes_supported published by the Shopify Customer Account OIDC discovery document served\n  on cuyana.com. customer-account-mcp-api:full is the scope gating the Customer Account MCP\n  surface.\nschemes:\n- name: ShopifyCustomerAccountOAuth\n  source: well-known/cuyana-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.cuyana.com/authentication/oauth/authorize\n    tokenUrl: https://account.cuyana.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (issue an ID token).\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account\
  \ API for the authenticated customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API surface.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuyana/refs/heads/main/scopes/cuyana-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Fashion
- Retail
- E-commerce
- Direct-to-Consumer
- Apparel
- Leather Goods
- Sustainable Fashion
- Shopify
token_urls:
- https://account.cuyana.com/authentication/oauth/token
---
