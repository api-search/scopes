---
authorization_urls:
- https://shopify.com/authentication/30430134331/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Primary Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Primary publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Primary API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/30430134331/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Primary
provider_slug: primary
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/30430134331/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/30430134331/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/primary-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OIDC authentication; issue an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven customer operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: primary-scopes
source_filename: primary-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://www.primary.com/.well-known/oauth-authorization-server\n  (scopes_supported) — Shopify Customer Account API\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/primary-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/30430134331/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/30430134331/oauth/token\nscopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token for the signed-in customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account\
  \ MCP API for agent-driven customer operations.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primary/refs/heads/main/scopes/primary-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Retail
- Ecommerce
- Apparel
- Children
- Shopify
- Agent
token_urls:
- https://shopify.com/authentication/30430134331/oauth/token
---
