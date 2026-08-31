---
authorization_urls:
- https://shopify.com/authentication/3466100806/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Olipop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Olipop publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Olipop API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/3466100806/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Olipop
provider_slug: olipop
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/3466100806/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/3466100806/oauth/token
  issuer: https://shopify.com/authentication/3466100806
  name: shopifyCustomerAccounts
  source: well-known/olipop-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the authenticated customer - orders, addresses, subscriptions and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API, the agent-facing projection of the customer account surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: olipop-scopes
source_filename: olipop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://drinkolipop.com/.well-known/openid-configuration\nnotes: >-\n  The only OAuth scope surface on the OLIPOP domain is the Shopify customer-accounts authorization server\n  advertised at /.well-known/openid-configuration (and identically at /.well-known/oauth-authorization-server)\n  for shop id 3466100806. There is no developer-facing OAuth app program and no per-resource scope\n  taxonomy; scopes_supported below is the verbatim published list. The UCP/MCP commerce endpoint does not\n  use OAuth scopes at all - it gates on a UCP platform agent profile plus human buyer approval.\nschemes:\n- name: shopifyCustomerAccounts\n  type: openIdConnect\n  source: well-known/olipop-openid-configuration.json\n  issuer: https://shopify.com/authentication/3466100806\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/3466100806/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/3466100806/oauth/token\n\
  \    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/olipop-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/olipop-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the authenticated customer -\n    orders, addresses, subscriptions and profile.\n  flows: [authorizationCode]\n  sources: [well-known/olipop-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API, the agent-facing projection of the\n    customer account surface.\n  flows: [authorizationCode]\n  sources: [well-known/olipop-openid-configuration.json]\nx-evidence:\n  fetched: '2026-07-31'\n \
  \ url: https://drinkolipop.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olipop/refs/heads/main/scopes/olipop-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- beverage
- consumer-packaged-goods
- direct-to-consumer
- E-Commerce
- Retail
- agent-commerce
- universal-commerce-protocol
- MCP
- graphql
- shopify
- prebiotic-soda
- functional-beverage
token_urls:
- https://shopify.com/authentication/3466100806/oauth/token
---
