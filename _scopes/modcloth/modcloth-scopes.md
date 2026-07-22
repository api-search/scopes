---
authorization_urls:
- https://account.modcloth.com/authentication/oauth/authorize
description: ''
docs: https://modcloth.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Modcloth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Modcloth publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Modcloth API on a user''s behalf.


  Tokens are issued from https://account.modcloth.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Modcloth
provider_slug: modcloth
schemes:
- flows:
  - authorizationUrl: https://account.modcloth.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.modcloth.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/55906042027
  name: shopify-customer-account-oidc
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect — issue an ID token for the authenticated shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Access the shopper's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in shopper (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — agent access to the shopper's account context.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: modcloth-scopes
source_filename: modcloth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://modcloth.com/.well-known/openid-configuration\ndocs: https://modcloth.com/.well-known/oauth-authorization-server\nschemes:\n- name: shopify-customer-account-oidc\n  issuer: https://shopify.com/authentication/55906042027\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.modcloth.com/authentication/oauth/authorize\n    tokenUrl: https://account.modcloth.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token for the authenticated shopper.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the shopper's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in shopper (orders, profile, addresses).\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description:\
  \ Full access to the Customer Account MCP API — agent access to the shopper's account context.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modcloth/refs/heads/main/scopes/modcloth-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-commerce
- Fashion
- Apparel
- Shopify
- Agentic Commerce
- MCP
token_urls:
- https://account.modcloth.com/authentication/oauth/token
---
