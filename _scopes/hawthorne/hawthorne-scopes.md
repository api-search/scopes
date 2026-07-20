---
authorization_urls:
- https://shopify.com/authentication/57105744010/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hawthorne Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hawthorne publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hawthorne API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/57105744010/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hawthorne
provider_slug: hawthorne
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/57105744010/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/57105744010/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/hawthorne-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows: []
  scope: openid
- description: Access the authenticated customer's email address.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface (agent-driven commerce).
  flows: []
  scope: customer-account-mcp-api:full
slug: hawthorne-scopes
source_filename: hawthorne-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://hawthorne.co/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth/OIDC scopes advertised by the store's Shopify Customer Account API\n  discovery document. These are Shopify platform scopes surfaced on the Hawthorne\n  shop host, not a bespoke Hawthorne scope registry. The customer-account-mcp-api\n  scope gates the store's agent-facing MCP commerce endpoint.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/hawthorne-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/57105744010/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/57105744010/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  sources: [well-known/hawthorne-openid-configuration.json]\n- scope: email\n  description: Access the authenticated\
  \ customer's email address.\n  sources: [well-known/hawthorne-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  sources: [well-known/hawthorne-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface (agent-driven commerce).\n  sources: [well-known/hawthorne-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawthorne/refs/heads/main/scopes/hawthorne-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Consumer Goods
- Personal Care
- Grooming
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/57105744010/oauth/token
---
