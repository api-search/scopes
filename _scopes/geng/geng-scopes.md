---
authorization_urls:
- https://shopify.com/authentication/55492378809/oauth/authorize
description: ''
docs: https://geng.gg/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Geng Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gen.G publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gen.G API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/55492378809/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gen.G
provider_slug: geng
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/55492378809/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/55492378809/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/geng-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: geng-scopes
source_filename: geng-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://geng.gg/.well-known/openid-configuration\ndocs: https://geng.gg/.well-known/openid-configuration\nnotes: >-\n  Scopes advertised by the Shopify Customer Account API OpenID Connect\n  discovery document served under the geng.gg storefront domain\n  (scopes_supported). These govern customer-account login for the Gen.G store,\n  not a first-party Gen.G developer API.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/geng-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/55492378809/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/55492378809/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication.\n    flows: [authorizationCode]\n    sources: [well-known/geng-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's email address and\
  \ verification status.\n    flows: [authorizationCode]\n    sources: [well-known/geng-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/geng-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/geng-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geng/refs/heads/main/scopes/geng-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Esports
- Gaming
- Entertainment
- Media
- Sports
token_urls:
- https://shopify.com/authentication/55492378809/oauth/token
---
