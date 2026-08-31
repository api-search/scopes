---
api_specs:
- filename: hyperice-collections-api-openapi.yml
  format: yaml
  label: Hyperice Collections API
  slug: hyperice-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-collections-api-openapi.yml
- filename: hyperice-discovery-api-openapi.yml
  format: yaml
  label: Hyperice Discovery API
  slug: hyperice-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-discovery-api-openapi.yml
- filename: hyperice-products-api-openapi.yml
  format: yaml
  label: Hyperice Products API
  slug: hyperice-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-products-api-openapi.yml
authorization_urls:
- https://accounts.hyperice.com/authentication/oauth/authorize
description: 'The complete OAuth scope surface Hyperice advertises, taken verbatim from the scopes_supported array of the OIDC discovery document served on its own domain. Four scopes, all coarse-grained: two OIDC standard scopes and two full-access product scopes. There is no fine-grained read/write scope split and no per-resource scoping.'
docs: https://hyperice.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Hyperice Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hyperice publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hyperice API on a user''s behalf.


  Tokens are issued from https://accounts.hyperice.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hyperice
provider_slug: hyperice
schemes:
- flows:
  - authorizationUrl: https://accounts.hyperice.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://accounts.hyperice.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/78618525910
  name: HypericeCustomerAccounts
  source: well-known/hyperice-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OIDC scope. Authenticates the buyer and requests an ID token carrying the iss, sub, aud, exp, iat, nonce and sid claims.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope. Releases the buyer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: 'Full access to the Customer Account API on behalf of the signed-in buyer — profile, addresses, orders, subscriptions. Coarse-grained: there is no read-only or per-resource variant advertised.'
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API on behalf of the signed-in buyer. This is the scope that lets an agent act against buyer-owned data over MCP, and it is the highest-consequence grant on the perimeter.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: hyperice-scopes
source_filename: hyperice-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://hyperice.com/.well-known/openid-configuration\ndescription: >-\n  The complete OAuth scope surface Hyperice advertises, taken verbatim from the\n  scopes_supported array of the OIDC discovery document served on its own\n  domain. Four scopes, all coarse-grained: two OIDC standard scopes and two\n  full-access product scopes. There is no fine-grained read/write scope split\n  and no per-resource scoping.\ndocs: https://hyperice.com/.well-known/openid-configuration\nschemes:\n- name: HypericeCustomerAccounts\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/78618525910\n  source: well-known/hyperice-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.hyperice.com/authentication/oauth/authorize\n    tokenUrl: https://accounts.hyperice.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: >-\n    Standard OIDC scope.\
  \ Authenticates the buyer and requests an ID token\n    carrying the iss, sub, aud, exp, iat, nonce and sid claims.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [well-known/hyperice-openid-configuration.json]\n- scope: email\n  description: >-\n    Standard OIDC scope. Releases the buyer's email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [well-known/hyperice-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Customer Account API on behalf of the signed-in buyer —\n    profile, addresses, orders, subscriptions. Coarse-grained: there is no\n    read-only or per-resource variant advertised.\n  granularity: full\n  flows: [authorizationCode]\n  sources: [well-known/hyperice-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API on behalf of the signed-in\n    buyer.\
  \ This is the scope that lets an agent act against buyer-owned data\n    over MCP, and it is the highest-consequence grant on the perimeter.\n  granularity: full\n  flows: [authorizationCode]\n  sources: [well-known/hyperice-openid-configuration.json]\nobservations:\n- >-\n  All four scopes are advertised identically by both /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server — the two documents are\n  byte-identical on this store.\n- >-\n  Neither product scope offers a least-privilege alternative. An agent that only\n  needs to read order status must request the same :full grant as one that can\n  mutate the buyer's profile.\n- >-\n  The public read tier (products/collections JSON, Storefront GraphQL) requires\n  no scope at all, so the scope surface applies solely to buyer-scoped\n  operations.\nx-evidence:\n  fetched: '2026-07-31'\n  probes:\n  - {url: 'https://hyperice.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://hyperice.com/.well-known/oauth-authorization-server',\
  \ http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/scopes/hyperice-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- Retail
- Health and Wellness
- Consumer Hardware
- Sports And Fitness
- Agentic Commerce
- GraphQL
- MCP
- Shopify
token_urls:
- https://accounts.hyperice.com/authentication/oauth/token
---
