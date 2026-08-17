---
authorization_urls:
- https://shopify.com/authentication/1157103680/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Centric Brands Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Centric Brands publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Centric Brands API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/1157103680/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Centric Brands
provider_slug: centric-brands
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/1157103680/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/1157103680/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/centric-brands-openid-configuration.json
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
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer (orders, addresses, profile) for that brand store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface, the authenticated counterpart to the anonymous UCP shopping tools.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: centric-brands-scopes
source_filename: centric-brands-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.hudsonjeans.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  scopes_supported advertised by the authorization servers behind Centric\n  Brands' owned-brand storefronts (Shopify Customer Accounts). Identical on all\n  eight probed hosts, with a per-store issuer. There is no corporate Centric\n  Brands OAuth server; these scopes govern buyer-delegated access to a single\n  brand store, not company data.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/centric-brands-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/1157103680/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/1157103680/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the buyer.\n    flows:\n      - authorizationCode\n\
  \    sources:\n      - well-known/centric-brands-openid-configuration.json\n  - scope: email\n    description: Access the buyer's email address claim.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/centric-brands-openid-configuration.json\n  - scope: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the\n      signed-in buyer (orders, addresses, profile) for that brand store.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/centric-brands-openid-configuration.json\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the Customer Account MCP API surface, the authenticated\n      counterpart to the anonymous UCP shopping tools.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/centric-brands-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centric-brands/refs/heads/main/scopes/centric-brands-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Apparel
- Accessories
- Footwear
- Beauty
- Kids
- Lifestyle
- Brand Management
- Licensing
- Entertainment Licensing
- Sports Licensing
- Fashion
- Consumer Products
- Fortune 1000
- Private Equity Owned
token_urls:
- https://shopify.com/authentication/1157103680/oauth/token
---
