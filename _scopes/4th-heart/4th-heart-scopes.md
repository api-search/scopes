---
authorization_urls:
- https://shopify.com/authentication/6414473/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 4Th Heart Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from scopes_supported in the merchant's own OAuth 2.0 authorization-server and OpenID Connect discovery documents. Descriptions below are the plain reading of each scope name; 4th & Heart publishes no scope reference page of its own, because the authorization server is operated by Shopify on the merchant's behalf. The agent-commerce MCP endpoint at /api/ucp/mcp is anonymous and consumes none of these scopes.
overview: '4th & Heart publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 4th & Heart API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/6414473/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 4th & Heart
provider_slug: 4th-heart
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/6414473/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/6414473/oauth/token
  issuer: https://shopify.com/authentication/6414473
  name: shopify-customer-account
  source: well-known/4th-heart-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an OpenID Connect ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and its verification state.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the signed-in customer's account data via the Customer Account API.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API, the authenticated counterpart to the anonymous storefront commerce MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: 4th-heart-scopes
source_filename: 4th-heart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://fourthandheart.com/.well-known/openid-configuration\nnote: >-\n  Scopes read verbatim from scopes_supported in the merchant's own OAuth 2.0 authorization-server and\n  OpenID Connect discovery documents. Descriptions below are the plain reading of each scope name;\n  4th & Heart publishes no scope reference page of its own, because the authorization server is\n  operated by Shopify on the merchant's behalf. The agent-commerce MCP endpoint at /api/ucp/mcp is\n  anonymous and consumes none of these scopes.\nschemes:\n- name: shopify-customer-account\n  issuer: https://shopify.com/authentication/6414473\n  source: well-known/4th-heart-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/6414473/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/6414473/oauth/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect\
  \ ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/4th-heart-openid-configuration.json]\n- scope: email\n  description: Release the customer's email address and its verification state.\n  flows: [authorizationCode]\n  sources: [well-known/4th-heart-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the signed-in customer's account data via the Customer Account API.\n  flows: [authorizationCode]\n  sources: [well-known/4th-heart-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API, the authenticated counterpart to the anonymous\n    storefront commerce MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/4th-heart-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4th-heart/refs/heads/main/scopes/4th-heart-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
token_urls:
- https://shopify.com/authentication/6414473/oauth/token
---
