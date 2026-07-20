---
authorization_urls:
- https://shopify.com/authentication/47328854173/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Holy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HOLY publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HOLY API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/47328854173/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HOLY
provider_slug: holy
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/47328854173/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/47328854173/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/holy-openid-configuration.json
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
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API (orders, profile, addresses) for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: holy-scopes
source_filename: holy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://de.holy.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/holy-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/47328854173/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/47328854173/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/holy-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/holy-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API (orders, profile, addresses) for the authenticated customer.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/holy-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/holy-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holy/refs/heads/main/scopes/holy-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Beverages
- Direct-to-Consumer
- Ecommerce
- Agentic Commerce
- Shopify
- Germany
token_urls:
- https://shopify.com/authentication/47328854173/oauth/token
---
