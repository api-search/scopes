---
api_specs:
- filename: liquid-death-catalog-api-openapi.yml
  format: yaml
  label: Liquid Death Catalog API
  slug: liquid-death-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-catalog-api-openapi.yml
- filename: liquid-death-discovery-api-openapi.yml
  format: yaml
  label: Liquid Death Discovery API
  slug: liquid-death-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-discovery-api-openapi.yml
authorization_urls:
- https://account.liquiddeath.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Liquid Death Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Liquid Death publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Liquid Death API on a user''s behalf.


  Tokens are issued from https://account.liquiddeath.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Liquid Death
provider_slug: liquid-death
schemes:
- flows:
  - authorizationUrl: https://account.liquiddeath.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce_required_methods:
    - S256
    tokenUrl: https://account.liquiddeath.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/7942897737
  name: customer-account-oidc
  source: well-known/liquid-death-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for this store on behalf of the signed-in customer (orders, addresses, subscriptions, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer account surface over MCP — the agent-mediated equivalent of customer-account-api:full. Its presence is what makes customer-scoped agent operations (e.g. get_order) possible alongside the anonymous UCP shopping transport.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: liquid-death-scopes
source_filename: liquid-death-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://liquiddeath.com/.well-known/openid-configuration\nsummary:\n  scheme_count: 1\n  scope_count: 4\n  note: >-\n    Scopes are taken verbatim from the scopes_supported array of the store's own OIDC/OAuth discovery\n    documents. Liquid Death publishes no separate scopes reference page; these four are the complete\n    advertised set.\nschemes:\n  - name: customer-account-oidc\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/7942897737\n    source: well-known/liquid-death-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.liquiddeath.com/authentication/oauth/authorize\n        tokenUrl: https://account.liquiddeath.com/authentication/oauth/token\n        pkce_required_methods: [S256]\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; requests an ID token identifying the customer.\n    flows: [authorizationCode]\n\
  \    sources: [well-known/liquid-death-openid-configuration.json, well-known/liquid-death-oauth-authorization-server.json]\n  - scope: email\n    description: Releases the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/liquid-death-openid-configuration.json, well-known/liquid-death-oauth-authorization-server.json]\n  - scope: 'customer-account-api:full'\n    description: >-\n      Full access to the customer account API for this store on behalf of the signed-in customer\n      (orders, addresses, subscriptions, profile).\n    flows: [authorizationCode]\n    sources: [well-known/liquid-death-openid-configuration.json, well-known/liquid-death-oauth-authorization-server.json]\n  - scope: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the customer account surface over MCP — the agent-mediated equivalent of\n      customer-account-api:full. Its presence is what makes customer-scoped agent operations\n\
  \      (e.g. get_order) possible alongside the anonymous UCP shopping transport.\n    flows: [authorizationCode]\n    sources: [well-known/liquid-death-openid-configuration.json, well-known/liquid-death-oauth-authorization-server.json]\ngaps:\n  - >-\n    No granular read/write scope decomposition is offered — both non-OIDC scopes are \":full\". An agent\n    that only needs order status must request the same authority as one that can mutate the account.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://liquiddeath.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/scopes/liquid-death-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
token_urls:
- https://account.liquiddeath.com/authentication/oauth/token
---
