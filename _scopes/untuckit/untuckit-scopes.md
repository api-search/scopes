---
authorization_urls: []
description: OAuth 2.0 / OIDC scopes published in the storefront's live OIDC discovery document (issuer https://shopify.com/authentication/1291072, saved at well-known/untuckit-openid-configuration.json). These are the Shopify Customer Account API scopes for the UNTUCKit store; the mcp scope grants customer-context access to the store's UCP/MCP agent-commerce endpoint.
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Untuckit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UNTUCKit publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the UNTUCKit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UNTUCKit
provider_slug: untuckit
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an id_token identifying the customer.
  flows: []
  scope: openid
- description: Access to the customer's email address and verification status claims.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for this store (orders, profile, addresses) on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API, allowing agents to act with customer context against the store's MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: untuckit-scopes
source_filename: untuckit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://untuckit.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  OAuth 2.0 / OIDC scopes published in the storefront's live OIDC discovery\n  document (issuer https://shopify.com/authentication/1291072, saved at\n  well-known/untuckit-openid-configuration.json). These are the Shopify\n  Customer Account API scopes for the UNTUCKit store; the mcp scope grants\n  customer-context access to the store's UCP/MCP agent-commerce endpoint.\nauthorization_server: https://account.untuckit.com/authentication/oauth/authorize\ntoken_endpoint: https://account.untuckit.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; returns an id_token identifying the customer.\n  - scope: email\n    description: Access to the customer's email address and verification status claims.\n  - scope: customer-account-api:full\n    description: Full\
  \ access to the Shopify Customer Account API for this store (orders, profile, addresses) on behalf of the signed-in customer.\n  - scope: customer-account-mcp-api:full\n    description: Full access to the customer-account MCP API, allowing agents to act with customer context against the store's MCP endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/untuckit/refs/heads/main/scopes/untuckit-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Apparel
- Retail
- eCommerce
- Shopify
- Agentic Commerce
- MCP
- UCP
token_urls: []
---
