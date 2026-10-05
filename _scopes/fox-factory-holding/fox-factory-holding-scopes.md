---
authorization_urls:
- https://shopify.com/authentication/68121624800/oauth/authorize
description: OAuth 2.0 / OpenID Connect scopes advertised by the customer-account authorization server behind the FOX storefront at ridefox.com. These are buyer-account scopes, not developer/partner API scopes — Fox Factory publishes no partner API scope reference. Scope descriptions below are our reading of the scope names; the discovery document publishes names only.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fox Factory Holding Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fox Factory Holding publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fox Factory Holding API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/68121624800/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fox Factory Holding
provider_slug: fox-factory-holding
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.
  flows: []
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the signed-in customer's account (orders, addresses, profile) via the Shopify Customer Account API.
  flows: []
  scope: customer-account-api:full
- description: Full access to the signed-in customer's account through the Customer Account MCP API — the buyer-scoped counterpart to the anonymous UCP commerce MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: fox-factory-holding-scopes
source_filename: fox-factory-holding-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://ridefox.com/.well-known/openid-configuration (HTTP 200, 2026-09-14)\nprovider: Fox Factory Holding\nproviderId: fox-factory-holding\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the customer-account authorization server behind the\n  FOX storefront at ridefox.com. These are buyer-account scopes, not developer/partner API scopes —\n  Fox Factory publishes no partner API scope reference. Scope descriptions below are our reading of the\n  scope names; the discovery document publishes names only.\nissuer: https://shopify.com/authentication/68121624800\nauthorization_endpoint: https://shopify.com/authentication/68121624800/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/68121624800/oauth/token\ndocs: null\ndocs_note: No first-party scope reference page is published on any Fox Factory host.\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests\
  \ an ID token for the signed-in customer.\n    standard: true\n  - name: email\n    description: Releases the customer's email address and email_verified claim.\n    standard: true\n  - name: customer-account-api:full\n    description: Full access to the signed-in customer's account (orders, addresses, profile) via the Shopify Customer Account API.\n    standard: false\n  - name: customer-account-mcp-api:full\n    description: Full access to the signed-in customer's account through the Customer Account MCP API — the buyer-scoped counterpart to the anonymous UCP commerce MCP endpoint.\n    standard: false\nobserved_in_the_wild:\n  - flow: storefront login\n    url: https://ridefox.com/customer_authentication/login\n    requested_scope: openid email customer-account-api\n    note: Observed on the 302 to the Shopify authorize endpoint (2026-09-14).\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ncode_challenge_methods_supported: [S256]\nmaintainers:\n  - FN:\
  \ Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-factory-holding/refs/heads/main/scopes/fox-factory-holding-scopes.yml
summary_line: 4 scopes
tags:
- Suspension
- Cycling
- Power-Sports
- Manufacturing
- E-Commerce
- MCP
- Agentic Commerce
token_bound: false
token_urls:
- https://shopify.com/authentication/68121624800/oauth/token
---
