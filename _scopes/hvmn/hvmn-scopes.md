---
authorization_urls:
- https://account.ketone.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hvmn Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HVMN publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HVMN API on a user''s behalf.


  Tokens are issued from https://account.ketone.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HVMN
provider_slug: hvmn
schemes:
- flows:
  - authorizationUrl: https://account.ketone.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.ketone.com/authentication/oauth/token
  name: ShopifyCustomerAccount
  source: well-known/hvmn-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
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
- description: Full access to the Shopify Customer Account MCP API for agent-driven access on behalf of the customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: hvmn-scopes
source_filename: hvmn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://ketone.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n  - name: ShopifyCustomerAccount\n    source: well-known/hvmn-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.ketone.com/authentication/oauth/authorize\n        tokenUrl: https://account.ketone.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; returns an ID token identifying the customer.\n    flows: [authorizationCode]\n    sources: [well-known/hvmn-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/hvmn-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n\
  \    flows: [authorizationCode]\n    sources: [well-known/hvmn-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for agent-driven access on behalf of the customer.\n    flows: [authorizationCode]\n    sources: [well-known/hvmn-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hvmn/refs/heads/main/scopes/hvmn-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Nutrition
- Ketones
- Supplements
- E-Commerce
- Shopify
- Agentic Commerce
- Consumer
- MCP
token_urls:
- https://account.ketone.com/authentication/oauth/token
---
