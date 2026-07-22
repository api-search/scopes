---
authorization_urls:
- https://shopify.com/authentication/61841768621/oauth/authorize
description: ''
docs: https://becausemarket.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Because Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Because publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Because API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/61841768621/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Because
provider_slug: because
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/61841768621/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/61841768621/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/because-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OIDC authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven customer-account actions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: because-scopes
source_filename: because-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://becausemarket.com/.well-known/openid-configuration\ndocs: https://becausemarket.com/.well-known/openid-configuration\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/because-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/61841768621/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/61841768621/oauth/token\nscopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token for the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/because-openid-configuration.json\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/because-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\
  \ customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/because-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agent-driven customer-account actions.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/because-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/because/refs/heads/main/scopes/because-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-commerce
- Health
- Incontinence
- Senior Care
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/61841768621/oauth/token
---
