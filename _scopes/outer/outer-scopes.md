---
authorization_urls:
- https://account.liveouter.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Outer Scopes
name_suffix: OAuth Scopes
note: Scopes taken verbatim from scopes_supported in the live discovery document served at liveouter.com. There is no OpenAPI to derive from; descriptions below describe what each scope name denotes in the Shopify Customer Account API and are not additional scopes.
overview: 'Outer publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outer API on a user''s behalf.


  Tokens are issued from https://account.liveouter.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outer
provider_slug: outer
schemes:
- flows:
  - authorizationUrl: https://account.liveouter.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.liveouter.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/11846615098
  name: ShopifyCustomerAccount
  source: well-known/outer-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the signed-in customer.
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
- description: Full access to the customer-account MCP API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: outer-scopes
source_filename: outer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://liveouter.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Scopes taken verbatim from scopes_supported in the live discovery document served at\n  liveouter.com. There is no OpenAPI to derive from; descriptions below describe what each\n  scope name denotes in the Shopify Customer Account API and are not additional scopes.\nschemes:\n- name: ShopifyCustomerAccount\n  source: well-known/outer-openid-configuration.json\n  issuer: https://shopify.com/authentication/11846615098\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.liveouter.com/authentication/oauth/authorize\n    tokenUrl: https://account.liveouter.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/outer-openid-configuration.json]\n\
  - scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/outer-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/outer-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/outer-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://liveouter.com/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outer/refs/heads/main/scopes/outer-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Furniture
- Home
- Direct to Consumer
- Agentic Commerce
- Shopify
- Universal Commerce Protocol
token_urls:
- https://account.liveouter.com/authentication/oauth/token
---
