---
authorization_urls:
- https://shopify.com/authentication/3860496433/oauth/authorize
description: ''
docs: https://bartesian.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bartesian Scopes
name_suffix: OAuth Scopes
note: Bartesian ships no OpenAPI, so these scopes were not derived from a spec. They are the scopes_supported list published verbatim by the Shopify customer account authorization server that fronts the Bartesian storefront (issuer https://shopify.com/authentication/3860496433). The UCP / MCP commerce endpoint at /api/ucp/mcp does not use these scopes - it identifies the calling platform with a UCP-Agent profile URI instead - so this scope set covers customer-account access only.
overview: 'Bartesian publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bartesian API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/3860496433/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bartesian
provider_slug: bartesian
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/3860496433/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/3860496433/oauth/token
  issuer: https://shopify.com/authentication/3860496433
  name: shopify-customer-account-oidc
  source: well-known/bartesian-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the signed-in Bartesian customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify customer-account MCP API for the signed-in customer - the authenticated, customer-scoped MCP surface, distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bartesian-scopes
source_filename: bartesian-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://bartesian.com/.well-known/openid-configuration\ndocs: https://bartesian.com/.well-known/oauth-authorization-server\nnote: >-\n  Bartesian ships no OpenAPI, so these scopes were not derived from a spec. They\n  are the scopes_supported list published verbatim by the Shopify customer\n  account authorization server that fronts the Bartesian storefront\n  (issuer https://shopify.com/authentication/3860496433). The UCP / MCP commerce\n  endpoint at /api/ucp/mcp does not use these scopes - it identifies the calling\n  platform with a UCP-Agent profile URI instead - so this scope set covers\n  customer-account access only.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/bartesian-openid-configuration.json\n  issuer: https://shopify.com/authentication/3860496433\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/3860496433/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/3860496433/oauth/token\n\
  \    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the\n    signed-in Bartesian customer.\n  flows: [authorizationCode]\n  sources: [well-known/bartesian-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/bartesian-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer\n    (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/bartesian-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify customer-account MCP API for the signed-in\n    customer - the authenticated, customer-scoped MCP surface, distinct from the\n    anonymous UCP shopping MCP endpoint at /api/ucp/mcp.\n  flows: [authorizationCode]\n  sources:\
  \ [well-known/bartesian-openid-configuration.json]\ngranularity:\n  assessment: coarse\n  note: >-\n    Two of the four scopes are `:full`. There is no read-only or per-resource\n    split (orders vs addresses vs subscriptions), so a customer authorizing an\n    agent to read order history necessarily grants write access to the whole\n    account. This is a Shopify platform default, not a Bartesian choice, but it\n    is the consent surface a Bartesian customer actually faces.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://bartesian.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bartesian/refs/heads/main/scopes/bartesian-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- Ecommerce
- Consumer Products
- Appliances
- Beverages
- Direct to Consumer
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/3860496433/oauth/token
---
