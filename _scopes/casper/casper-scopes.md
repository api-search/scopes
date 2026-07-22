---
authorization_urls:
- https://shopify.com/authentication/60822683729/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Casper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Casper publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Casper API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/60822683729/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Casper
provider_slug: casper
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/60822683729/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/60822683729/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/casper-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
  flows: []
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated buyer.
  flows: []
  scope: customer-account-api:full
- description: Full agentic (MCP) access to the Customer Account API on behalf of the buyer.
  flows: []
  scope: customer-account-mcp-api:full
slug: casper-scopes
source_filename: casper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://casper.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Scopes advertised by the Shopify Customer Account API OIDC discovery document for\n  the casper.com storefront. customer-account-mcp-api:full is the scope that grants\n  agentic (MCP) access to the customer account surface.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/casper-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/60822683729/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/60822683729/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer\
  \ Account API for the authenticated buyer.\n- scope: customer-account-mcp-api:full\n  description: Full agentic (MCP) access to the Customer Account API on behalf of the buyer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casper/refs/heads/main/scopes/casper-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ecommerce
- Retail
- Sleep
- Mattresses
- Direct to Consumer
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/60822683729/oauth/token
---
