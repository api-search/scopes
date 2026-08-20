---
authorization_urls:
- https://shopify.com/authentication/11195850/oauth/authorize
description: ''
docs: https://shop.bombas.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bombas Scopes
name_suffix: OAuth Scopes
note: Bombas ships no OpenAPI, so these scopes were not derived from a spec. They are the scopes_supported list published verbatim by the Shopify customer account authorization server that fronts the Bombas storefront (issuer https://shopify.com/authentication/11195850). The UCP / MCP commerce endpoint at /api/ucp/mcp does not use these scopes - it authenticates the calling platform with a UCP-Agent profile URI instead - so this scope set covers customer-account access only.
overview: 'Bombas publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bombas API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/11195850/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bombas
provider_slug: bombas
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/11195850/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/11195850/oauth/token
  issuer: https://shopify.com/authentication/11195850
  name: shopify-customer-account-oidc
  source: well-known/bombas-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the signed-in Bombas customer.
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
- description: Full access to the Shopify customer-account MCP API for the signed-in customer - the authenticated, customer-scoped MCP surface, distinct from the anonymous UCP shopping MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bombas-scopes
source_filename: bombas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://shop.bombas.com/.well-known/openid-configuration\ndocs: https://shop.bombas.com/.well-known/oauth-authorization-server\nnote: >-\n  Bombas ships no OpenAPI, so these scopes were not derived from a spec. They\n  are the scopes_supported list published verbatim by the Shopify customer\n  account authorization server that fronts the Bombas storefront\n  (issuer https://shopify.com/authentication/11195850). The UCP / MCP commerce\n  endpoint at /api/ucp/mcp does not use these scopes - it authenticates the\n  calling platform with a UCP-Agent profile URI instead - so this scope set\n  covers customer-account access only.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/bombas-openid-configuration.json\n  issuer: https://shopify.com/authentication/11195850\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/11195850/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/11195850/oauth/token\n\
  \    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the\n    signed-in Bombas customer.\n  flows: [authorizationCode]\n  sources: [well-known/bombas-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/bombas-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer\n    (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/bombas-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify customer-account MCP API for the signed-in\n    customer - the authenticated, customer-scoped MCP surface, distinct from the\n    anonymous UCP shopping MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/bombas-openid-configuration.json]\n\
  x-evidence:\n  fetched: '2026-07-31'\n  url: https://shop.bombas.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bombas/refs/heads/main/scopes/bombas-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Direct to Consumer
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
token_urls:
- https://shopify.com/authentication/11195850/oauth/token
---
