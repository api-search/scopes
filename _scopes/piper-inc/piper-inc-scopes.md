---
authorization_urls:
- https://shopify.com/authentication/9256256/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Piper Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Piper Inc. publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Piper Inc. API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/9256256/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Piper Inc.
provider_slug: piper-inc
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/9256256/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/9256256/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/piper-inc-openid-configuration.json
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
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on the buyer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: piper-inc-scopes
source_filename: piper-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.playpiper.in/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account Authentication\n  server for the Piper store (id 9256256), from scopes_supported in the OIDC\n  discovery document.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/piper-inc-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/9256256/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/9256256/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer\
  \ Account API on the buyer's behalf.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API for agent-driven commerce.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piper-inc/refs/heads/main/scopes/piper-inc-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Education
- EdTech
- STEM
- Hardware
- E-Commerce
- Agentic Commerce
- MCP
- Shopify
token_urls:
- https://shopify.com/authentication/9256256/oauth/token
---
