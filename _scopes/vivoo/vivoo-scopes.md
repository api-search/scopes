---
authorization_urls:
- https://shopify.com/authentication/85119664427/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Vivoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vivoo publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vivoo API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/85119664427/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vivoo
provider_slug: vivoo
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/85119664427/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/85119664427/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/vivoo-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Authenticate the customer and return an ID token (OpenID Connect).
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven interactions on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: vivoo-scopes
source_filename: vivoo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.vivoo.io/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/vivoo-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/85119664427/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/85119664427/oauth/token\nscopes:\n- scope: openid\n  description: Authenticate the customer and return an ID token (OpenID Connect).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/vivoo-openid-configuration.json\n- scope: email\n  description: Access the customer's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/vivoo-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\n    customer.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - well-known/vivoo-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for agent-driven\n    interactions on behalf of the signed-in customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/vivoo-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivoo/refs/heads/main/scopes/vivoo-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Wellness
- Consumer Health
- Nutrition
- Diagnostics
- E-Commerce
- Agentic Commerce
- MCP
token_urls:
- https://shopify.com/authentication/85119664427/oauth/token
---
