---
authorization_urls:
- https://shopify.com/authentication/60285812930/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Slingshot Biosciences Scopes
name_suffix: OAuth Scopes
note: There is no OpenAPI to derive scopes from. These are the scopes the store's own OAuth 2.0 / OIDC authorization server advertises in its RFC 8414 discovery document, captured verbatim at well-known/slingshot-biosciences-oauth-authorization-server.json. They govern customer-scoped access to the Customer Account API and the customer-scoped half of the MCP server; anonymous storefront reads need no scope at all.
overview: 'Slingshot Biosciences publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Slingshot Biosciences API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/60285812930/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Slingshot Biosciences
provider_slug: slingshot-biosciences
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/60285812930/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/60285812930/oauth/token
  issuer: https://shopify.com/authentication/60285812930
  name: shopify-customer-account
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an id_token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Customer Account API for the authenticated customer — orders, addresses, profile and subscriptions on the Slingshot Bio store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full customer-scoped access through the MCP server, letting an agent act on the authenticated customer's account rather than only the anonymous catalog.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: slingshot-biosciences-scopes
source_filename: slingshot-biosciences-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://slingshot-bio.myshopify.com/.well-known/oauth-authorization-server\nnote: >-\n  There is no OpenAPI to derive scopes from. These are the scopes the store's own\n  OAuth 2.0 / OIDC authorization server advertises in its RFC 8414 discovery\n  document, captured verbatim at\n  well-known/slingshot-biosciences-oauth-authorization-server.json. They govern\n  customer-scoped access to the Customer Account API and the customer-scoped half\n  of the MCP server; anonymous storefront reads need no scope at all.\nschemes:\n- name: shopify-customer-account\n  issuer: https://shopify.com/authentication/60285812930\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/60285812930/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/60285812930/oauth/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an id_token\
  \ identifying the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Customer Account API for the authenticated customer —\n    orders, addresses, profile and subscriptions on the Slingshot Bio store.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full customer-scoped access through the MCP server, letting an agent act on\n    the authenticated customer's account rather than only the anonymous catalog.\n  flows: [authorizationCode]\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://slingshot-bio.myshopify.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slingshot-biosciences/refs/heads/main/scopes/slingshot-biosciences-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Biotechnology
- Life Sciences
- Flow Cytometry
- Laboratory
- Synthetic Biology
- Diagnostics
- Cell Therapy
- E-Commerce
- GraphQL
- MCP
token_urls:
- https://shopify.com/authentication/60285812930/oauth/token
---
