---
authorization_urls:
- https://shopify.com/authentication/63533449453/oauth/authorize
description: ''
docs: https://thefolklore.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: The Folklore Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Shopify Customer Account authorization server that fronts The Folklore's storefront. Captured verbatim from the live discovery document's scopes_supported.
overview: 'The Folklore publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Folklore API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/63533449453/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Folklore
provider_slug: the-folklore
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/63533449453/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/63533449453/oauth/token
  issuer: https://shopify.com/authentication/63533449453
  name: shopifyCustomerAccountOIDC
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the agent-driven (UCP) commerce surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: the-folklore-scopes
source_filename: the-folklore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thefolklore.com/.well-known/openid-configuration\ndocs: https://thefolklore.com/.well-known/openid-configuration\nnote: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account authorization\n  server that fronts The Folklore's storefront. Captured verbatim from the live\n  discovery document's scopes_supported.\nschemes:\n- name: shopifyCustomerAccountOIDC\n  issuer: https://shopify.com/authentication/63533449453\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/63533449453/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/63533449453/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n \
  \ description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API — the agent-driven (UCP) commerce surface.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-folklore/refs/heads/main/scopes/the-folklore-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- Wholesale
- Marketplace
- Retail
- E-commerce
- Fashion
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/63533449453/oauth/token
---
