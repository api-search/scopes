---
authorization_urls:
- https://shopify.com/authentication/56172019867/oauth/authorize
description: ''
docs: https://chill.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Chill Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Chill publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chill API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/56172019867/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chill
provider_slug: chill
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/56172019867/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/56172019867/oauth/token
  name: ShopifyCustomerAccountOAuth
  source: well-known/chill-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication of the Shopify customer account
  flows: []
  scope: openid
- description: Access to the customer's email address and verification status
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer
  flows: []
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — enables agent-driven commerce (UCP) on behalf of the buyer
  flows: []
  scope: customer-account-mcp-api:full
slug: chill-scopes
source_filename: chill-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://chill.com/.well-known/openid-configuration\ndocs: https://chill.com/.well-known/openid-configuration\nschemes:\n- name: ShopifyCustomerAccountOAuth\n  source: well-known/chill-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/56172019867/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/56172019867/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the Shopify customer account\n- scope: email\n  description: Access to the customer's email address and verification status\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API — enables agent-driven commerce (UCP) on behalf of the buyer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chill/refs/heads/main/scopes/chill-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Wellness
- Supplements
- E-commerce
- Marketplace
- Health
- Agentic Commerce
- Shopify
- Retail
- MCP
token_urls:
- https://shopify.com/authentication/56172019867/oauth/token
---
