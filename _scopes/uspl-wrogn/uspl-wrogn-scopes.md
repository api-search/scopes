---
authorization_urls: []
description: OAuth scopes published in the store's own OIDC discovery document (Shopify Customer Accounts, issuer https://shopify.com/authentication/81803051309, served from https://wrogn.com/.well-known/openid-configuration and mirrored at /.well-known/oauth-authorization-server). scopes_supported captured verbatim; no additional scope reference is published by the brand itself.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Uspl Wrogn Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'USPL Wrogn publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the USPL Wrogn API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: USPL Wrogn
provider_slug: uspl-wrogn
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (standard OIDC scope).
  flows: []
  scope: openid
- description: Access to the customer's email address claim (standard OIDC scope).
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer (orders, profile, addresses) on this store.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-scoped MCP API surface, enabling authenticated agent operations against the storefront MCP server on behalf of the customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: uspl-wrogn-scopes
source_filename: uspl-wrogn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://wrogn.com/.well-known/openid-configuration\ndescription: >-\n  OAuth scopes published in the store's own OIDC discovery document\n  (Shopify Customer Accounts, issuer\n  https://shopify.com/authentication/81803051309, served from\n  https://wrogn.com/.well-known/openid-configuration and mirrored at\n  /.well-known/oauth-authorization-server). scopes_supported captured\n  verbatim; no additional scope reference is published by the brand itself.\nprovider: uspl-wrogn\nissuer: https://shopify.com/authentication/81803051309\nauthorization_endpoint: https://shopify.com/authentication/81803051309/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/81803051309/oauth/token\ngrant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\npkce: S256\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (standard OIDC scope).\n  - scope: email\n  \
  \  description: Access to the customer's email address claim (standard OIDC scope).\n  - scope: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API for the authenticated\n      customer (orders, profile, addresses) on this store.\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-scoped MCP API surface, enabling\n      authenticated agent operations against the storefront MCP server on\n      behalf of the customer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspl-wrogn/refs/heads/main/scopes/uspl-wrogn-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Consumer
- Fashion
- Apparel
- eCommerce
- Retail
- India
- Agentic Commerce
- MCP
token_urls: []
---
