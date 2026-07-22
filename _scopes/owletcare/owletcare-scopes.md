---
authorization_urls:
- https://b2b.owletcare.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Owletcare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Owletcare publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Owletcare API on a user''s behalf.


  Tokens are issued from https://b2b.owletcare.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Owletcare
provider_slug: owletcare
schemes:
- flows:
  - authorizationUrl: https://b2b.owletcare.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://b2b.owletcare.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/owletcare-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: owletcare-scopes
source_filename: owletcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://owletcare.com/.well-known/openid-configuration\nnotes: >-\n  Scopes advertised by the Shopify Customer Account OIDC discovery document\n  served at owletcare.com (scopes_supported). This is Shopify's Customer\n  Account API scope set, not a first-party Owlet API.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/owletcare-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://b2b.owletcare.com/authentication/oauth/authorize\n    tokenUrl: https://b2b.owletcare.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the authenticated customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n  flows: [authorizationCode]\n\
  - scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owletcare/refs/heads/main/scopes/owletcare-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Baby Care
- Health Monitoring
- Consumer Electronics
- Connected Devices
- IoT
- Sleep
- Wearables
token_urls:
- https://b2b.owletcare.com/authentication/oauth/token
---
