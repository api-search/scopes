---
authorization_urls:
- https://shopify.com/authentication/88395284786/oauth/authorize
- https://shopify.com/authentication/55874814054/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Harry S Scopes
name_suffix: OAuth Scopes
note: Scopes come from the scopes_supported array of the live OIDC / RFC 8414 discovery documents the two Shopify-hosted brands serve from their own domains. There is no OpenAPI to derive from and Mammoth Brands publishes no scope reference page, so descriptions below are the standard OIDC meanings plus the Shopify Customer Account API scope names verbatim — nothing was invented and no scope was added that the discovery document does not list.
overview: 'Mammoth Brands publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mammoth Brands API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/88395284786/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mammoth Brands
provider_slug: harry-s
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/88395284786/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/88395284786/oauth/token
  name: shopify-customer-account-oidc-harrys
  source: well-known/harry-s-harrys-openid-configuration.json
- flows:
  - authorizationUrl: https://shopify.com/authentication/55874814054/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/55874814054/oauth/token
  name: shopify-customer-account-oidc-flamingo
  source: well-known/harry-s-flamingo-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface on behalf of the signed-in customer — the authenticated counterpart to the anonymous storefront MCP server at /api/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: harry-s-scopes
source_filename: harry-s-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://harrys.com/.well-known/openid-configuration\nnote: >-\n  Scopes come from the scopes_supported array of the live OIDC / RFC 8414 discovery documents\n  the two Shopify-hosted brands serve from their own domains. There is no OpenAPI to derive\n  from and Mammoth Brands publishes no scope reference page, so descriptions below are the\n  standard OIDC meanings plus the Shopify Customer Account API scope names verbatim — nothing\n  was invented and no scope was added that the discovery document does not list.\nschemes:\n- name: shopify-customer-account-oidc-harrys\n  source: well-known/harry-s-harrys-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/88395284786/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/88395284786/oauth/token\n    pkce: S256\n- name: shopify-customer-account-oidc-flamingo\n  source: well-known/harry-s-flamingo-openid-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/55874814054/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/55874814054/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/harry-s-harrys-openid-configuration.json, well-known/harry-s-flamingo-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/harry-s-harrys-openid-configuration.json, well-known/harry-s-flamingo-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/harry-s-harrys-openid-configuration.json,\
  \ well-known/harry-s-flamingo-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface on behalf of the signed-in customer — the\n    authenticated counterpart to the anonymous storefront MCP server at /api/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/harry-s-harrys-openid-configuration.json, well-known/harry-s-flamingo-openid-configuration.json]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ndocs: null\ndocs_note: Mammoth Brands publishes no developer documentation for these scopes; the discovery document is the only source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harry-s/refs/heads/main/scopes/harry-s-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Retail
- E-Commerce
- Personal Care
- Agentic Commerce
- Model Context Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/88395284786/oauth/token
- https://shopify.com/authentication/55874814054/oauth/token
---
