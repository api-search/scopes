---
authorization_urls:
- https://shopify.com/authentication/83104301340/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jubilee Tv Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jubilee TV publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jubilee TV API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/83104301340/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jubilee TV
provider_slug: jubilee-tv
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/83104301340/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/83104301340/oauth/token
  name: ShopifyCustomerAccountsOIDC
  source: well-known/jubilee-tv-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication of the customer identity
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated customer's email address
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the customer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven access
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: jubilee-tv-scopes
source_filename: jubilee-tv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://getjubileetv.com/.well-known/openid-configuration\nnotes: >-\n  OAuth 2.0 / OIDC scopes advertised by the Shopify Customer Accounts\n  authorization server for the getjubileetv.com storefront. These are the\n  platform-provided customer-account scopes (including the agentic\n  customer-account MCP scope), not scopes on a bespoke Jubilee TV developer API.\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  source: well-known/jubilee-tv-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/83104301340/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/83104301340/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the customer identity\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the authenticated customer's email address\n  flows: [authorizationCode]\n- scope: 'customer-account-api:full'\n\
  \  description: Full access to the Shopify Customer Account API on behalf of the customer\n  flows: [authorizationCode]\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the Shopify Customer Account MCP API for agent-driven access\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jubilee-tv/refs/heads/main/scopes/jubilee-tv-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Caregiving
- Seniors
- Smart TV
- Video Calling
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/83104301340/oauth/token
---
