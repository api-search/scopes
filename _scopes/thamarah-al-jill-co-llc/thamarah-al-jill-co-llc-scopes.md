---
authorization_urls:
- https://shopify.com/authentication/29798400044/oauth/authorize
description: ''
docs: https://amusedco.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Thamarah Al Jill Co Llc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Thamarah Al-Jill Co LLC publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thamarah Al-Jill Co LLC API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/29798400044/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thamarah Al-Jill Co LLC
provider_slug: thamarah-al-jill-co-llc
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/29798400044/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/29798400044/oauth/token
  name: shopify-customer-accounts-oidc
  source: well-known/thamarah-al-jill-co-llc-openid-configuration.json
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
- description: Full access to the Customer Account MCP API — agent-facing customer-account operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: thamarah-al-jill-co-llc-scopes
source_filename: thamarah-al-jill-co-llc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://amusedco.com/.well-known/openid-configuration\ndocs: https://amusedco.com/.well-known/openid-configuration\nschemes:\n  - name: shopify-customer-accounts-oidc\n    source: well-known/thamarah-al-jill-co-llc-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/29798400044/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/29798400044/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the buyer.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access the buyer's email address claim.\n    flows: [authorizationCode]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.\n    flows: [authorizationCode]\n  - scope: customer-account-mcp-api:full\n    description: Full\
  \ access to the Customer Account MCP API — agent-facing customer-account operations.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thamarah-al-jill-co-llc/refs/heads/main/scopes/thamarah-al-jill-co-llc-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-commerce
- Marketplace
- Luxury
- Resale
- Fashion
- Agent Commerce
- Shopify
- Saudi Arabia
token_urls:
- https://shopify.com/authentication/29798400044/oauth/token
---
