---
authorization_urls:
- https://accounts.allbirds.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Allbirds Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allbirds publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allbirds API on a user''s behalf.


  Tokens are issued from https://accounts.allbirds.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allbirds
provider_slug: allbirds
schemes:
- flows:
  - authorizationUrl: https://accounts.allbirds.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.allbirds.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/allbirds-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the buyer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: allbirds-scopes
source_filename: allbirds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.allbirds.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth 2.0 / OIDC scopes advertised by Allbirds's Shopify Customer Accounts\n  authorization server (scopes_supported in the discovery documents). Descriptions\n  reflect the Shopify Customer Account API and its MCP surface.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/allbirds-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.allbirds.com/authentication/oauth/authorize\n        tokenUrl: https://accounts.allbirds.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the buyer.\n    flows: [authorizationCode]\n    sources: [well-known/allbirds-openid-configuration.json]\n  - scope: email\n    description: Access the buyer's email address claim.\n\
  \    flows: [authorizationCode]\n    sources: [well-known/allbirds-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.\n    flows: [authorizationCode]\n    sources: [well-known/allbirds-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Customer Account MCP API surface for agent-driven commerce.\n    flows: [authorizationCode]\n    sources: [well-known/allbirds-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allbirds/refs/heads/main/scopes/allbirds-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Retail
- E-commerce
- Footwear
- Apparel
- Sustainability
- Direct-to-Consumer
- Agent Commerce
- Shopify
token_urls:
- https://accounts.allbirds.com/authentication/oauth/token
---
