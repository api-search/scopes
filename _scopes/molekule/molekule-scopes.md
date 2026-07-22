---
authorization_urls:
- https://shopify.com/authentication/70884294938/oauth/authorize
description: OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC discovery document served from molekule.com. These gate buyer-account and customer-account MCP access for the storefront.
docs: https://molekule.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Molekule Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Molekule publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Molekule API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/70884294938/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Molekule
provider_slug: molekule
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/70884294938/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/70884294938/oauth/token
  name: shopifyCustomerAccountOIDC
  source: well-known/molekule-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the buyer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven flows.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: molekule-scopes
source_filename: molekule-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: well-known/molekule-openid-configuration.json\ndocs: https://molekule.com/.well-known/openid-configuration\ndescription: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC\n  discovery document served from molekule.com. These gate buyer-account and\n  customer-account MCP access for the storefront.\nschemes:\n- name: shopifyCustomerAccountOIDC\n  source: well-known/molekule-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/70884294938/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/70884294938/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the buyer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the buyer's email address claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to\
  \ the Shopify Customer Account API for the signed-in buyer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agent-driven flows.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/molekule/refs/heads/main/scopes/molekule-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Hardware
- Air Quality
- Consumer IoT
- E-Commerce
- Agent Commerce
- MCP
- Shopify
token_urls:
- https://shopify.com/authentication/70884294938/oauth/token
---
