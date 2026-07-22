---
authorization_urls:
- https://shopify.com/authentication/69929140544/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rouje Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC discovery fronting Rouje's storefront. Not a Rouje-specific scope registry.
overview: 'Rouje publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rouje API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/69929140544/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rouje
provider_slug: rouje
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/69929140544/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/69929140544/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/rouje-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication of the customer/buyer
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email and email_verified claim
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the buyer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven interactions
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: rouje-scopes
source_filename: rouje-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.rouje.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC discovery\n  fronting Rouje's storefront. Not a Rouje-specific scope registry.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/rouje-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/69929140544/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/69929140544/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the customer/buyer\n  flows: [authorizationCode]\n  sources: [well-known/rouje-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email and email_verified claim\n  flows: [authorizationCode]\n  sources: [well-known/rouje-openid-configuration.json]\n- scope: customer-account-api:full\n\
  \  description: Full access to the Shopify Customer Account API on behalf of the buyer\n  flows: [authorizationCode]\n  sources: [well-known/rouje-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API for agent-driven interactions\n  flows: [authorizationCode]\n  sources: [well-known/rouje-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rouje/refs/heads/main/scopes/rouje-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Fashion
- Beauty
- Retail
- Ecommerce
- Shopify
- Agentic Commerce
- Paris
token_urls:
- https://shopify.com/authentication/69929140544/oauth/token
---
