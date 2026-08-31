---
authorization_urls: []
description: The only scope surface Supergoop! exposes is the scopes_supported list on its customer-accounts OIDC discovery document, served from supergoop.com and backed by the Shopify-hosted authorization server for shop 15035658. There is no developer-facing OAuth app registration and no published scope reference page, so this list is the whole of it.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Supergoop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Supergoop! uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Supergoop!
provider_slug: supergoop
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: supergoop-scopes
source_filename: supergoop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://supergoop.com/.well-known/openid-configuration\ndescription: >-\n  The only scope surface Supergoop! exposes is the scopes_supported list on its\n  customer-accounts OIDC discovery document, served from supergoop.com and backed\n  by the Shopify-hosted authorization server for shop 15035658. There is no\n  developer-facing OAuth app registration and no published scope reference page,\n  so this list is the whole of it.\nauthorization_server: https://shopify.com/authentication/15035658\ndiscovery: https://supergoop.com/.well-known/openid-configuration\ngrant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\npkce_methods: [S256]\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OIDC scope; requests an ID token for the signed-in shopper.\n    standard: true\n  - name: email\n    description: Releases the shopper's email and email_verified claims.\n    standard:\
  \ true\n  - name: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API for the signed-in shopper —\n      orders, addresses, subscriptions and profile for that customer only.\n    standard: false\n  - name: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-account MCP API. This is the scope an agent\n      acting for a signed-in shopper would hold; it is the credential path behind\n      the get_order tool on the UCP MCP server, which returns\n      AuthenticationRequired when called anonymously.\n    standard: false\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ndocs: null\ndocs_note: >-\n  Supergoop! publishes no scope reference. Scope semantics are documented by the\n  platform at https://shopify.dev/docs/api/customer, which is Shopify's page, not\n  Supergoop!'s — recorded here rather than cited as a provider document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supergoop/refs/heads/main/scopes/supergoop-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Sunscreen
- Skincare
- Beauty
- Cosmetics
- Consumer Goods
- Retail
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- GraphQL
token_urls: []
---
