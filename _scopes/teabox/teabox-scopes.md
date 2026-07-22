---
authorization_urls:
- https://accounts.teabox.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Teabox Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Teabox (Shopify Customer Account API) authorization server. Includes the customer-account MCP scope that gates the UCP agent-commerce MCP endpoint.
overview: 'Teabox publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Teabox API on a user''s behalf.


  Tokens are issued from https://accounts.teabox.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Teabox
provider_slug: teabox
schemes:
- flows:
  - authorizationUrl: https://accounts.teabox.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.teabox.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/teabox-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the buyer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the buyer's Shopify Customer Account API (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface for agent-driven commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: teabox-scopes
source_filename: teabox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.teabox.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  OAuth/OIDC scopes advertised by the Teabox (Shopify Customer Account API)\n  authorization server. Includes the customer-account MCP scope that gates the\n  UCP agent-commerce MCP endpoint.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/teabox-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.teabox.com/authentication/oauth/authorize\n    tokenUrl: https://accounts.teabox.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the buyer.\n  flows: [authorizationCode]\n  sources: [well-known/teabox-openid-configuration.json]\n- scope: email\n  description: Access the buyer's email address and verification status.\n  flows: [authorizationCode]\n  sources: [well-known/teabox-openid-configuration.json]\n\
  - scope: customer-account-api:full\n  description: Full access to the buyer's Shopify Customer Account API (orders, profile, addresses).\n  flows: [authorizationCode]\n  sources: [well-known/teabox-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface for agent-driven commerce.\n  flows: [authorizationCode]\n  sources: [well-known/teabox-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teabox/refs/heads/main/scopes/teabox-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Tea
- Food and Beverage
- E-commerce
- Retail
- Shopify
- Agent Commerce
token_urls:
- https://accounts.teabox.com/authentication/oauth/token
---
