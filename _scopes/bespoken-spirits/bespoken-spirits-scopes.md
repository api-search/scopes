---
authorization_urls:
- https://shopify.com/authentication/75681399024/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bespoken Spirits Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bespoken Spirits publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bespoken Spirits API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/75681399024/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bespoken Spirits
provider_slug: bespoken-spirits
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/75681399024/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/75681399024/oauth/token
  issuer: https://shopify.com/authentication/75681399024
  name: shopify-customer-account-oidc
  source: well-known/bespoken-spirits-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OIDC scope requesting an ID token for the authenticated buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the buyer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the authenticated buyer — orders, addresses, profile and subscriptions for this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API — the authenticated, buyer-scoped counterpart to the anonymous storefront MCP endpoints catalogued in mcp/bespoken-spirits-mcp.yml.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bespoken-spirits-scopes
source_filename: bespoken-spirits-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://bespokenspirits.com/.well-known/openid-configuration\nnotes: >-\n  These are the OAuth 2.0 / OIDC scopes advertised by the Shopify Customer Account\n  authorization server bound to the bespokenspirits.com storefront. They are read\n  verbatim from scopes_supported in the store's own /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server documents. Bespoken Spirits publishes no\n  scope reference page of its own; the descriptions below are the standard meanings of\n  the scope names, not provider-authored copy.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/bespoken-spirits-openid-configuration.json\n  issuer: https://shopify.com/authentication/75681399024\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/75681399024/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/75681399024/oauth/token\n    pkce: S256\n\
  scopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated buyer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/bespoken-spirits-openid-configuration.json\n- scope: email\n  description: Release the buyer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/bespoken-spirits-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the\n    authenticated buyer — orders, addresses, profile and subscriptions for this store.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/bespoken-spirits-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API — the authenticated,\n    buyer-scoped counterpart to the anonymous storefront MCP endpoints catalogued in\n    mcp/bespoken-spirits-mcp.yml.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - well-known/bespoken-spirits-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://bespokenspirits.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://bespokenspirits.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoken-spirits/refs/heads/main/scopes/bespoken-spirits-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Spirits
- Beverage Alcohol
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Retail
- Manufacturing
token_urls:
- https://shopify.com/authentication/75681399024/oauth/token
---
