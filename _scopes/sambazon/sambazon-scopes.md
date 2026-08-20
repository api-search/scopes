---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised in the customer-account authorization-server metadata that www.sambazon.com publishes. These are Shopify platform scopes surfaced on the merchant origin — SAMBAZON does not define its own scope vocabulary, and the UCP/MCP endpoint at /api/ucp/mcp is not scope-gated (it is gated on an agent profile URI instead, see ../authentication/sambazon-authentication.yml).
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sambazon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sambazon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sambazon
provider_slug: sambazon
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sambazon-scopes
source_filename: sambazon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://www.sambazon.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised in the customer-account\n  authorization-server metadata that www.sambazon.com publishes. These are\n  Shopify platform scopes surfaced on the merchant origin — SAMBAZON does not\n  define its own scope vocabulary, and the UCP/MCP endpoint at /api/ucp/mcp is\n  not scope-gated (it is gated on an agent profile URI instead, see\n  ../authentication/sambazon-authentication.yml).\nissuer: https://shopify.com/authentication/52008485056\nflows:\n  authorization_code:\n    authorizationUrl: https://shopify.com/authentication/52008485056/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/52008485056/oauth/token\n    pkce: S256\n    refresh: supported\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope. Requests an ID token\
  \ identifying the\n      signed-in shopper.\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: >-\n      Standard OpenID Connect scope. Releases the email and email_verified\n      claims for the signed-in shopper.\n    standard: OpenID Connect Core 1.0\n  - name: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the\n      signed-in shopper — their orders, addresses, payment methods and profile\n      for this store.\n    standard: Shopify platform scope\n  - name: customer-account-mcp-api:full\n    description: >-\n      Full access to the Shopify Customer Account MCP API on behalf of the\n      signed-in shopper. This is the authenticated, customer-scoped counterpart\n      to the anonymous UCP/MCP commerce endpoint — it is how an agent acts on a\n      logged-in buyer's own account data rather than on the public catalog.\n    standard: Shopify platform scope\ncoverage:\n  scopes_declared: 4\n  scopes_openid_standard:\
  \ 2\n  scopes_platform: 2\nnotes:\n  - >-\n    scopes_supported is the only scope surface published. There is no\n    per-operation scope mapping, because no OpenAPI is published for this\n    origin.\n  - >-\n    token_endpoint_auth_methods_supported is client_secret_basic only, and the\n    jwt-bearer grant is also offered — both Shopify platform behaviours.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://www.sambazon.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambazon/refs/heads/main/scopes/sambazon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Retail
- Sustainability
token_urls: []
---
