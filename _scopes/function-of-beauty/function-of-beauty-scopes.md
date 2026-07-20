---
authorization_urls:
- https://shopify.com/authentication/69081399608/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Function Of Beauty Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the Shopify Customer Account API OpenID Connect discovery document served on the Function of Beauty domain (scopes_supported). Captured verbatim; descriptions are from Shopify's Customer Account API documentation.
overview: 'Function of Beauty publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Function of Beauty API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/69081399608/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Function of Beauty
provider_slug: function-of-beauty
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/69081399608/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/69081399608/oauth/token
  name: shopifyCustomerAccount
  source: well-known/function-of-beauty-openid-configuration.json
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
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: function-of-beauty-scopes
source_filename: function-of-beauty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://functionofbeauty.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Scopes advertised by the Shopify Customer Account API OpenID Connect discovery\n  document served on the Function of Beauty domain (scopes_supported). Captured\n  verbatim; descriptions are from Shopify's Customer Account API documentation.\nschemes:\n- name: shopifyCustomerAccount\n  source: well-known/function-of-beauty-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/69081399608/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/69081399608/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/function-of-beauty/refs/heads/main/scopes/function-of-beauty-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Beauty
- Personal Care
- Personalization
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
token_urls:
- https://shopify.com/authentication/69081399608/oauth/token
---
