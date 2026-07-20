---
authorization_urls:
- https://shopify.com/authentication/77478658352/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ami Paris Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AMI Paris publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AMI Paris API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/77478658352/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AMI Paris
provider_slug: ami-paris
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/77478658352/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/77478658352/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/ami-paris-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven customer actions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: ami-paris-scopes
source_filename: ami-paris-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.amiparis.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/ami-paris-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/77478658352/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/77478658352/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agent-driven customer\
  \ actions.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ami-paris/refs/heads/main/scopes/ami-paris-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Fashion
- Retail
- Ecommerce
- Shopify
- Agent Commerce
- UCP
token_urls:
- https://shopify.com/authentication/77478658352/oauth/token
---
