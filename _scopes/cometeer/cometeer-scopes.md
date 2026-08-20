---
api_specs:
- filename: cometeer-storefront-openapi.yml
  format: yaml
  label: Cometeer Storefront (read-only)
  slug: storefront
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/openapi/cometeer-storefront-openapi.yml
authorization_urls:
- https://shopify.com/authentication/74101293355/oauth/authorize
description: ''
docs: https://cometeer.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cometeer Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the `scopes_supported` array published by the authorization-server metadata served on Cometeer's own apex host. Cometeer publishes no separate scope reference page — it is a direct-to-consumer storefront, so the OAuth surface exists for shopper sign-in to the Cometeer account/subscription portal rather than for third-party API authorization. Descriptions below are the standard meanings of these identifiers; the provider does not publish prose for them.
overview: 'Cometeer publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cometeer API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/74101293355/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cometeer
provider_slug: cometeer
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/74101293355/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/74101293355/oauth/token
  issuer: https://shopify.com/authentication/74101293355
  name: CometeerCustomerAccountOIDC
  source: well-known/cometeer-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the shopper's `email` and `email_verified` claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated shopper's own customer account data (orders, subscriptions, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated shopper's customer account through the MCP agent interface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: cometeer-scopes
source_filename: cometeer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://cometeer.com/.well-known/openid-configuration\ndocs: https://cometeer.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are read verbatim from the `scopes_supported` array published by the\n  authorization-server metadata served on Cometeer's own apex host. Cometeer\n  publishes no separate scope reference page — it is a direct-to-consumer\n  storefront, so the OAuth surface exists for shopper sign-in to the Cometeer\n  account/subscription portal rather than for third-party API authorization.\n  Descriptions below are the standard meanings of these identifiers; the\n  provider does not publish prose for them.\nschemes:\n- name: CometeerCustomerAccountOIDC\n  source: well-known/cometeer-openid-configuration.json\n  issuer: https://shopify.com/authentication/74101293355\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/74101293355/oauth/authorize\n    tokenUrl:\
  \ https://shopify.com/authentication/74101293355/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the shopper.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [well-known/cometeer-openid-configuration.json]\n- scope: email\n  description: Releases the shopper's `email` and `email_verified` claims.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [well-known/cometeer-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated shopper's own customer account data (orders, subscriptions, addresses).\n  standard: Shopify Customer Account API\n  flows: [authorizationCode]\n  sources: [well-known/cometeer-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated shopper's customer account through the MCP agent interface.\n  standard: Shopify\
  \ Customer Account MCP API\n  flows: [authorizationCode]\n  sources: [well-known/cometeer-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://cometeer.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/scopes/cometeer-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Coffee
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Subscription
- Agentic Commerce
- Shopify
- MCP
token_urls:
- https://shopify.com/authentication/74101293355/oauth/token
---
