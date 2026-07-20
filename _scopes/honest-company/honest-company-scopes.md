---
authorization_urls:
- https://shopify.com/authentication/64768475320/oauth/authorize
description: ''
docs: https://honest.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Honest Company Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Honest Company publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Honest Company API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/64768475320/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Honest Company
provider_slug: honest-company
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/64768475320/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/64768475320/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/honest-company-openid-configuration.json
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
- description: Access the shopper's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated shopper.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full agent/MCP access to the Customer Account API for the authenticated shopper.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: honest-company-scopes
source_filename: honest-company-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://honest.com/.well-known/openid-configuration\ndocs: https://honest.com/.well-known/oauth-authorization-server\nnotes: >-\n  OAuth2 scopes advertised by the Shopify Customer Account API authorization\n  server that honest.com delegates authentication to. Captured verbatim from the\n  live OIDC discovery document's scopes_supported. Note the\n  customer-account-mcp-api scope, which authorizes agent/MCP access to the\n  customer account surface.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/honest-company-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/64768475320/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/64768475320/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/honest-company-openid-configuration.json]\n\
  - scope: email\n  description: Access the shopper's email address.\n  flows: [authorizationCode]\n  sources: [well-known/honest-company-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated shopper.\n  flows: [authorizationCode]\n  sources: [well-known/honest-company-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full agent/MCP access to the Customer Account API for the authenticated shopper.\n  flows: [authorizationCode]\n  sources: [well-known/honest-company-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honest-company/refs/heads/main/scopes/honest-company-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Goods
- E-commerce
- Retail
- Baby Care
- Personal Care
- Beauty
- Shopify
- Agentic Commerce
- MCP
- UCP
token_urls:
- https://shopify.com/authentication/64768475320/oauth/token
---
