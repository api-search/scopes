---
authorization_urls:
- https://shopify.com/authentication/54968025206/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Abcoffee Scopes
name_suffix: OAuth Scopes
note: abcoffee publishes no OpenAPI, so these scopes are read verbatim from the OpenID Connect discovery document served at abcoffee.in. The authorization server is the Shopify Customer Account platform hosted for this store (issuer https://shopify.com/authentication/54968025206).
overview: 'Abcoffee publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Abcoffee API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/54968025206/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Abcoffee
provider_slug: abcoffee
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/54968025206/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/54968025206/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/abcoffee-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer - orders, addresses, payment methods and subscription/profile data for this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API - the agent-facing projection of the customer account surface, which is what an agent needs to read a buyer's own orders through the MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: abcoffee-scopes
source_filename: abcoffee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://abcoffee.in/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  abcoffee publishes no OpenAPI, so these scopes are read verbatim from the OpenID Connect discovery\n  document served at abcoffee.in. The authorization server is the Shopify Customer Account platform\n  hosted for this store (issuer https://shopify.com/authentication/54968025206).\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/abcoffee-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/54968025206/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/54968025206/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/abcoffee-openid-configuration.json]\n- scope: email\n  description:\
  \ Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/abcoffee-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the signed-in customer - orders, addresses,\n    payment methods and subscription/profile data for this store.\n  flows: [authorizationCode]\n  sources: [well-known/abcoffee-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API - the agent-facing projection of the customer account\n    surface, which is what an agent needs to read a buyer's own orders through the MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/abcoffee-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcoffee/refs/heads/main/scopes/abcoffee-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Coffee
- Food and Beverage
- Retail
- Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
- India
- Subscriptions
token_urls:
- https://shopify.com/authentication/54968025206/oauth/token
---
