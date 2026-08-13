---
authorization_urls:
- https://account.davidprotein.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: probed
name: David Protein Scopes
name_suffix: OAuth Scopes
note: Probed from the live OpenID Connect / RFC 8414 discovery documents rather than derived from an OpenAPI - David publishes no spec. Four scopes are advertised; two of them are coarse ":full" grants, so an agent that needs order status alone cannot ask for less than full customer-account access.
overview: 'David Protein publishes 4 OAuth 2.0 scopes via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the David Protein API on a user''s behalf.


  Tokens are issued from https://account.davidprotein.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: David Protein
provider_slug: david-protein
schemes:
- flows:
  - authorizationUrl: https://account.davidprotein.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.davidprotein.com/authentication/oauth/token
  - flow: refreshToken
    tokenUrl: https://account.davidprotein.com/authentication/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://account.davidprotein.com/authentication/oauth/token
  name: customer-account-oauth
  source: well-known/david-protein-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP server at account.davidprotein.com/customer/api/mcp - order status, store credit balances and return requests.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: david-protein-scopes
source_filename: david-protein-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://davidprotein.com/.well-known/openid-configuration\nnote: >-\n  Probed from the live OpenID Connect / RFC 8414 discovery documents rather than derived\n  from an OpenAPI - David publishes no spec. Four scopes are advertised; two of them are\n  coarse \":full\" grants, so an agent that needs order status alone cannot ask for less\n  than full customer-account access.\nschemes:\n- name: customer-account-oauth\n  source: well-known/david-protein-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.davidprotein.com/authentication/oauth/authorize\n    tokenUrl: https://account.davidprotein.com/authentication/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://account.davidprotein.com/authentication/oauth/token\n  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    tokenUrl: https://account.davidprotein.com/authentication/oauth/token\nscopes:\n- scope: openid\n\
  \  description: OpenID Connect authentication; returns an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/david-protein-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/david-protein-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: Full access to the customer account API for the signed-in customer.\n  flows: [authorizationCode]\n  granularity: coarse\n  sources: [well-known/david-protein-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account MCP server at\n    account.davidprotein.com/customer/api/mcp - order status, store credit balances and\n    return requests.\n  flows: [authorizationCode]\n  granularity: coarse\n  sources: [well-known/david-protein-openid-configuration.json]\nobserved_in_the_wild:\n  note: >-\n    The storefront login\
  \ redirect requests scope \"openid email customer-account-api:full\",\n    confirming the authorization-code flow is live.\n  url: https://davidprotein.com/account/login\n  status: 200\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://davidprotein.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/david-protein/refs/heads/main/scopes/david-protein-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Agents
- MCP
- Universal Commerce Protocol
- Commerce
- E-Commerce
- Shopping
- Catalog
- Checkout
- Nutrition
- Food and Beverage
- Consumer Packaged Goods
- Shopify
token_urls:
- https://account.davidprotein.com/authentication/oauth/token
---
