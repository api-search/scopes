---
authorization_urls:
- https://account.candyclub.com/authentication/oauth/authorize
description: ''
docs: https://candyclub.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Candyclub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CandyClub publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CandyClub API on a user''s behalf.


  Tokens are issued from https://account.candyclub.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CandyClub
provider_slug: candyclub
schemes:
- flows:
  - authorizationUrl: https://account.candyclub.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.candyclub.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/candyclub-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven commerce (UCP shopping endpoint).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: candyclub-scopes
source_filename: candyclub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://candyclub.com/.well-known/openid-configuration\ndocs: https://candyclub.com/.well-known/openid-configuration\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/candyclub-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.candyclub.com/authentication/oauth/authorize\n        tokenUrl: https://account.candyclub.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issues an ID token for the customer.\n    flows: [authorizationCode]\n    sources: [well-known/candyclub-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/candyclub-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account\
  \ API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/candyclub-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Customer Account MCP API for agent-driven commerce (UCP shopping endpoint).\n    flows: [authorizationCode]\n    sources: [well-known/candyclub-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candyclub/refs/heads/main/scopes/candyclub-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Candy
- Confectionery
- Ecommerce
- Subscription
- Retail
- Shopify
- Agent Commerce
- UCP
token_urls:
- https://account.candyclub.com/authentication/oauth/token
---
