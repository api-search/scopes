---
authorization_urls:
- https://accounts.awaytravel.com/authentication/oauth/authorize
description: ''
docs: https://www.awaytravel.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Away Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Away publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Away API on a user''s behalf.


  Tokens are issued from https://accounts.awaytravel.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Away
provider_slug: away
schemes:
- flows:
  - authorizationUrl: https://accounts.awaytravel.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.awaytravel.com/authentication/oauth/token
  name: ShopifyCustomerAccounts
  source: well-known/away-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the buyer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP (agent-commerce) API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: away-scopes
source_filename: away-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.awaytravel.com/.well-known/openid-configuration\ndocs: https://www.awaytravel.com/.well-known/oauth-authorization-server\nschemes:\n- name: ShopifyCustomerAccounts\n  source: well-known/away-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.awaytravel.com/authentication/oauth/authorize\n    tokenUrl: https://accounts.awaytravel.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token for the buyer.\n  flows: [authorizationCode]\n  sources: [well-known/away-openid-configuration.json]\n- scope: email\n  description: Access the buyer's email address and verification status.\n  flows: [authorizationCode]\n  sources: [well-known/away-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.\n  flows:\
  \ [authorizationCode]\n  sources: [well-known/away-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP (agent-commerce) API for the signed-in buyer.\n  flows: [authorizationCode]\n  sources: [well-known/away-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/away/refs/heads/main/scopes/away-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Travel
- Retail
- E-commerce
- Luggage
- Agent Commerce
- Shopify
- MCP
token_urls:
- https://accounts.awaytravel.com/authentication/oauth/token
---
