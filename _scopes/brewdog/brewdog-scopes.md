---
authorization_urls:
- https://shopify.com/authentication/82272813382/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Brewdog Scopes
name_suffix: OAuth Scopes
note: BrewDog publishes no OpenAPI, so these scopes were not derived from oauth2 securitySchemes. They are the scopes_supported array of the OIDC discovery document BrewDog serves from its own origin for its Shopify Customer Account identity provider. No provider-published scope reference page was found.
overview: 'BrewDog publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BrewDog API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/82272813382/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BrewDog
provider_slug: brewdog
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/82272813382/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/82272813382/oauth/token
  issuer: https://shopify.com/authentication/82272813382
  name: shopify-customer-account-oidc
  source: well-known/brewdog-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in BrewDog customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in BrewDog customer (orders, addresses, profile, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer — the authenticated, account-scoped agent surface that sits alongside the anonymous UCP shopping MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: brewdog-scopes
source_filename: brewdog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://brewdog.com/.well-known/openid-configuration\nnote: BrewDog publishes no OpenAPI, so these scopes were not derived from oauth2\n  securitySchemes. They are the scopes_supported array of the OIDC discovery document\n  BrewDog serves from its own origin for its Shopify Customer Account identity\n  provider. No provider-published scope reference page was found.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/brewdog-openid-configuration.json\n  issuer: https://shopify.com/authentication/82272813382\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/82272813382/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/82272813382/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the signed-in\n    BrewDog customer.\n  flows: [authorizationCode]\n  sources: [well-known/brewdog-openid-configuration.json]\n\
  - scope: email\n  description: Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/brewdog-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the\n    signed-in BrewDog customer (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/brewdog-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API on behalf of the\n    signed-in customer — the authenticated, account-scoped agent surface that sits\n    alongside the anonymous UCP shopping MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/brewdog-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://brewdog.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brewdog/refs/heads/main/scopes/brewdog-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Beer
- Brewing
- Retail
- eCommerce
- Consumer Packaged Goods
- Hospitality
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/82272813382/oauth/token
---
