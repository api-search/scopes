---
authorization_urls:
- https://shopify.com/authentication/59465728192/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Voyage Foods Scopes
name_suffix: OAuth Scopes
note: Scopes are not derived from an OpenAPI (Voyage Foods publishes none). They are read verbatim from the scopes_supported array of the OIDC discovery / RFC 8414 authorization-server metadata document the storefront serves at voyagefoods.com/.well-known/. Descriptions below state what each scope gates on the Shopify Customer Accounts issuer that backs this storefront; the storefront itself publishes no scope reference page.
overview: 'Voyage Foods publishes 4 OAuth 2.0 scopes via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Voyage Foods API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/59465728192/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Voyage Foods
provider_slug: voyage-foods
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/59465728192/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token
  - flow: refreshToken
    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token
  issuer: https://shopify.com/authentication/59465728192
  name: ShopifyCustomerAccountsOIDC
  source: well-known/voyage-foods-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim in the ID token.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer — orders, addresses, profile and subscription data for this shop.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated, customer-scoped MCP surface, distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: voyage-foods-scopes
source_filename: voyage-foods-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://voyagefoods.com/.well-known/openid-configuration\nnote: >-\n  Scopes are not derived from an OpenAPI (Voyage Foods publishes none). They are read verbatim from\n  the scopes_supported array of the OIDC discovery / RFC 8414 authorization-server metadata document\n  the storefront serves at voyagefoods.com/.well-known/. Descriptions below state what each scope\n  gates on the Shopify Customer Accounts issuer that backs this storefront; the storefront itself\n  publishes no scope reference page.\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  issuer: https://shopify.com/authentication/59465728192\n  source: well-known/voyage-foods-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/59465728192/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token\n    pkce: S256\n  - flow: refreshToken\n    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token\n\
  \  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    tokenUrl: https://shopify.com/authentication/59465728192/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/voyage-foods-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email address and email_verified claim in the ID token.\n  flows: [authorizationCode]\n  sources: [well-known/voyage-foods-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in customer — orders,\n    addresses, profile and subscription data for this shop.\n  flows: [authorizationCode]\n  sources: [well-known/voyage-foods-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the Customer Account MCP API — the authenticated,\
  \ customer-scoped MCP surface,\n    distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/voyage-foods-openid-configuration.json]\nnot_scope_gated:\n- surface: https://voyagefoods.com/api/2026-04/graphql.json\n  reason: Public storefront reads are anonymous; no OAuth scope is presented.\n- surface: https://voyagefoods.com/api/ucp/mcp\n  reason: >-\n    UCP tool access is gated on an agent profile URI (meta.ucp-agent.profile), not on OAuth scopes.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://voyagefoods.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  scopes_supported_returned: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyage-foods/refs/heads/main/scopes/voyage-foods-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- Food Technology
token_urls:
- https://shopify.com/authentication/59465728192/oauth/token
---
