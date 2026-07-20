---
authorization_urls:
- https://shopify.com/authentication/7814423/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bloomthis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BloomThis publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BloomThis API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/7814423/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BloomThis
provider_slug: bloomthis
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/7814423/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/7814423/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/bloomthis-openid-configuration.json
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
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven customer operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bloomthis-scopes
source_filename: bloomthis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bloomthis.co/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/bloomthis-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/7814423/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/7814423/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/bloomthis-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows: [authorizationCode]\n  sources: [well-known/bloomthis-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/bloomthis-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agent-driven customer operations.\n  flows: [authorizationCode]\n  sources: [well-known/bloomthis-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomthis/refs/heads/main/scopes/bloomthis-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Flowers
- Gifting
- Ecommerce
- Retail
- Shopify
- Agent Commerce
- MCP
- Malaysia
token_urls:
- https://shopify.com/authentication/7814423/oauth/token
---
