---
authorization_urls:
- https://shopify.com/authentication/60989898907/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Virtuix Scopes
name_suffix: OAuth Scopes
note: Derived from no OpenAPI — Virtuix publishes none. These are the scopes the OIDC discovery document served on Virtuix's own host advertises for its Shopify customer-account authorization server.
overview: 'Virtuix publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virtuix API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/60989898907/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virtuix
provider_slug: virtuix
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/60989898907/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/60989898907/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/virtuix-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the storefront customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the storefront Customer Account API for the authenticated Virtuix shopper.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface — the scope that lets an agent act on the shopper's own account against the Virtuix store rather than only the anonymous catalog.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: virtuix-scopes
source_filename: virtuix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.virtuix.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  Derived from no OpenAPI — Virtuix publishes none. These are the scopes the OIDC discovery document\n  served on Virtuix's own host advertises for its Shopify customer-account authorization server.\nschemes:\n  - name: shopify-customer-account-oidc\n    source: well-known/virtuix-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/60989898907/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/60989898907/oauth/token\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; requests an ID token for the storefront customer.\n    flows: [authorizationCode]\n    sources: [well-known/virtuix-openid-configuration.json]\n  - scope: email\n    description: Releases the customer's email address and email_verified\
  \ claim.\n    flows: [authorizationCode]\n    sources: [well-known/virtuix-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the storefront Customer Account API for the authenticated Virtuix shopper.\n    flows: [authorizationCode]\n    sources: [well-known/virtuix-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-account MCP surface — the scope that lets an agent act on the\n      shopper's own account against the Virtuix store rather than only the anonymous catalog.\n    flows: [authorizationCode]\n    sources: [well-known/virtuix-openid-configuration.json]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuix/refs/heads/main/scopes/virtuix-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Virtual Reality
- Gaming
- Hardware
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Esports
- Game Development
- Location Based Entertainment
- Consumer Electronics
token_urls:
- https://shopify.com/authentication/60989898907/oauth/token
---
