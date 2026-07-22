---
authorization_urls:
- https://shopify.com/authentication/1501528/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Anine Bing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Anine Bing publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Anine Bing API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/1501528/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anine Bing
provider_slug: anine-bing
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/1501528/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/1501528/oauth/token
  issuer: https://shopify.com/authentication/1501528
  name: shopify-customer-account-oidc
  source: well-known/anine-bing-openid-configuration.json
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
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven customer operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: anine-bing-scopes
source_filename: anine-bing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://aninebing.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/anine-bing-openid-configuration.json\n  issuer: https://shopify.com/authentication/1501528\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/1501528/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/1501528/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: ['well-known/anine-bing-openid-configuration.json']\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: ['well-known/anine-bing-openid-configuration.json']\n- scope: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account\
  \ API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: ['well-known/anine-bing-openid-configuration.json']\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the Customer Account MCP API surface for agent-driven customer operations.\n  flows: [authorizationCode]\n  sources: ['well-known/anine-bing-openid-configuration.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anine-bing/refs/heads/main/scopes/anine-bing-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- Fashion
- Apparel
- Ecommerce
- Shopify
- Agent Commerce
- MCP
token_urls:
- https://shopify.com/authentication/1501528/oauth/token
---
