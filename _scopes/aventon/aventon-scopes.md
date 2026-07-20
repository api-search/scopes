---
authorization_urls:
- https://shopify.com/authentication/15202468/oauth/authorize
description: ''
docs: https://www.aventon.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Aventon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aventon publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aventon API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/15202468/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aventon
provider_slug: aventon
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/15202468/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/15202468/oauth/token
  name: shopifyCustomerAccountOIDC
  source: well-known/aventon-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API - the agent/MCP commerce surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: aventon-scopes
source_filename: aventon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.aventon.com/.well-known/openid-configuration\ndocs: https://www.aventon.com/.well-known/oauth-authorization-server\nnotes: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account authorization\n  server on aventon.com. customer-account-mcp-api:full is the scope that unlocks\n  the agent/MCP commerce surface documented in /llms.txt.\nschemes:\n- name: shopifyCustomerAccountOIDC\n  source: well-known/aventon-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/15202468/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/15202468/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the authenticated customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n\
  \  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API - the agent/MCP commerce surface.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aventon/refs/heads/main/scopes/aventon-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Electric Bikes
- E-Commerce
- Retail
- Agent Commerce
- Shopify
- Universal Commerce Protocol
token_urls:
- https://shopify.com/authentication/15202468/oauth/token
---
