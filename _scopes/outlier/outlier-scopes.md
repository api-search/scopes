---
authorization_urls:
- https://shopify.com/authentication/40681930915/oauth/authorize
description: ''
docs: https://www.outlier.org/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Outlier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Outlier publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outlier API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/40681930915/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outlier
provider_slug: outlier
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/40681930915/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/40681930915/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/outlier-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect sign-in; issue an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven interactions on behalf of the customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: outlier-scopes
source_filename: outlier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.outlier.org/.well-known/openid-configuration\ndocs: https://www.outlier.org/.well-known/openid-configuration\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/outlier-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/40681930915/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/40681930915/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token identifying the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/outlier-openid-configuration.json\n- scope: email\n  description: Access the customer's email address claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/outlier-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the customer.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - well-known/outlier-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API for agent-driven\n    interactions on behalf of the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/outlier-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outlier/refs/heads/main/scopes/outlier-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Education
- Online Learning
- Dual Enrollment
- E-Commerce
- Shopify
- Agent Commerce
- MCP
token_urls:
- https://shopify.com/authentication/40681930915/oauth/token
---
