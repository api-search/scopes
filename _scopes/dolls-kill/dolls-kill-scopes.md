---
authorization_urls:
- https://account.dollskill.com/authentication/oauth/authorize
description: ''
docs: https://www.dollskill.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Dolls Kill Scopes
name_suffix: OAuth Scopes
note: Not derived from OpenAPI — Dolls Kill publishes none. These scopes were read verbatim from the scopes_supported array of the live OpenID Connect discovery document the storefront serves, confirmed identical on the RFC 8414 authorization-server metadata document and observed again in the live login redirect from https://account.dollskill.com/.
overview: 'Dolls Kill publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dolls Kill API on a user''s behalf.


  Tokens are issued from https://account.dollskill.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dolls Kill
provider_slug: dolls-kill
schemes:
- flows:
  - authorizationUrl: https://account.dollskill.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.dollskill.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/63463358721
  name: Customer Account OAuth 2.0
  source: https://www.dollskill.com/.well-known/openid-configuration
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
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer — orders, addresses, payment methods and profile. Observed in the live login redirect issued by account.dollskill.com, which requests openid+email+customer-account-api:full.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated, customer-scoped counterpart to the anonymous UCP commerce MCP endpoint at /api/ucp/mcp. This is the scope an agent would need to read a buyer's own order history rather than only transact on the public catalog.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: dolls-kill-scopes
source_filename: dolls-kill-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://www.dollskill.com/.well-known/openid-configuration\ndocs: https://www.dollskill.com/.well-known/oauth-authorization-server\nnote: 'Not derived from OpenAPI — Dolls Kill publishes none. These scopes were read\n  verbatim from the scopes_supported array of the live OpenID Connect discovery document\n  the storefront serves, confirmed identical on the RFC 8414 authorization-server\n  metadata document and observed again in the live login redirect from\n  https://account.dollskill.com/.'\nschemes:\n- name: Customer Account OAuth 2.0\n  source: https://www.dollskill.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/63463358721\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.dollskill.com/authentication/oauth/authorize\n    tokenUrl: https://account.dollskill.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID\
  \ Connect scope; requests an ID token identifying the\n    signed-in customer.\n  flows: [authorizationCode]\n  sources: ['https://www.dollskill.com/.well-known/openid-configuration']\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: ['https://www.dollskill.com/.well-known/openid-configuration']\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated\n    customer — orders, addresses, payment methods and profile. Observed in the live\n    login redirect issued by account.dollskill.com, which requests openid+email+customer-account-api:full.\n  flows: [authorizationCode]\n  sources: ['https://www.dollskill.com/.well-known/openid-configuration']\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API — the authenticated,\n    customer-scoped counterpart to the anonymous UCP commerce MCP endpoint\
  \ at\n    /api/ucp/mcp. This is the scope an agent would need to read a buyer's own order\n    history rather than only transact on the public catalog.\n  flows: [authorizationCode]\n  sources: ['https://www.dollskill.com/.well-known/openid-configuration']\nscope_count: 4\nobservations:\n- 'The scope surface is coarse — both API scopes are :full, with no read/write or\n  per-resource split. An agent granted customer-account-api:full receives the whole\n  customer record.'\n- 'The public UCP commerce MCP endpoint requires no OAuth scope at all; it is gated\n  on a UCP agent profile URI instead. OAuth applies only to customer-account surfaces.'\nx-evidence:\n- url: https://www.dollskill.com/.well-known/openid-configuration\n  status: 200\n- url: https://account.dollskill.com/\n  status: 200\n  note: redirects to /authentication/login with scope=openid+email+customer-account-api%3Afull\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolls-kill/refs/heads/main/scopes/dolls-kill-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-commerce
- Fashion
- Apparel
- Commerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Direct to Consumer
token_urls:
- https://account.dollskill.com/authentication/oauth/token
---
