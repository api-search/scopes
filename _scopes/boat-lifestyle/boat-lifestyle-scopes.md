---
authorization_urls:
- https://shopify.com/authentication/5789384802/oauth/authorize
description: ''
docs: https://www.boat-lifestyle.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Boat Lifestyle Scopes
name_suffix: OAuth Scopes
note: Scopes are published in the OIDC/RFC 8414 discovery document served from the boAt Lifestyle storefront host. There is no OpenAPI declaring oauth2 securitySchemes; this is the authoritative published scope list for the surface.
overview: 'Boat Lifestyle publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Boat Lifestyle API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/5789384802/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Boat Lifestyle
provider_slug: boat-lifestyle
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/5789384802/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/5789384802/oauth/token
  issuer: https://shopify.com/authentication/5789384802
  name: ShopifyCustomerAccountsOIDC
  source: well-known/boat-lifestyle-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the buyer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the authenticated buyer — orders, addresses, profile and payment methods.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the buyer-scoped Customer Account MCP API, the authenticated counterpart to the anonymous commerce MCP endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: boat-lifestyle-scopes
source_filename: boat-lifestyle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://www.boat-lifestyle.com/.well-known/openid-configuration\ndocs: https://www.boat-lifestyle.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are published in the OIDC/RFC 8414 discovery document served from the boAt\n  Lifestyle storefront host. There is no OpenAPI declaring oauth2 securitySchemes;\n  this is the authoritative published scope list for the surface.\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  source: well-known/boat-lifestyle-openid-configuration.json\n  issuer: https://shopify.com/authentication/5789384802\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/5789384802/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/5789384802/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token for the authenticated\n    buyer.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - well-known/boat-lifestyle-openid-configuration.json\n- scope: email\n  description: Releases the buyer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/boat-lifestyle-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the authenticated\n    buyer — orders, addresses, profile and payment methods.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/boat-lifestyle-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the buyer-scoped Customer Account MCP API, the authenticated\n    counterpart to the anonymous commerce MCP endpoint at /api/ucp/mcp.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/boat-lifestyle-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-08'\n  url: https://www.boat-lifestyle.com/.well-known/openid-configuration\n  http_status: 200\n  content_type:\
  \ application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boat-lifestyle/refs/heads/main/scopes/boat-lifestyle-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Electronics
- E-Commerce
- Retail
- Audio
- Wearables
- Agent Commerce
- MCP
- Shopify
- India
token_urls:
- https://shopify.com/authentication/5789384802/oauth/token
---
