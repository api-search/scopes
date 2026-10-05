---
authorization_urls:
- https://shopify.com/authentication/67598516522/oauth/authorize
description: ''
docs: ''
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: probed
name: Hni Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the scopes_supported array of the authorization server metadata served at hearthnhome.com. HNI publishes no scope reference page; the authorization server is operated by Shopify. No OpenAPI exists, so derive-oauth-scopes.py produced nothing and this file was written from the live discovery document instead.
overview: 'HNI publishes 4 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HNI API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/67598516522/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HNI
provider_slug: hni
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect — request an ID token identifying the signed-in customer.
  flows: []
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer of the hearthnhome.com store.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API for the signed-in customer — the authenticated counterpart to the anonymous UCP commerce endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: hni-scopes
source_filename: hni-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://hearthnhome.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are read verbatim from the scopes_supported array of the authorization server metadata served\n  at hearthnhome.com. HNI publishes no scope reference page; the authorization server is operated by\n  Shopify. No OpenAPI exists, so derive-oauth-scopes.py produced nothing and this file was written from\n  the live discovery document instead.\nissuer: https://shopify.com/authentication/67598516522\nflows:\n  authorization_code:\n    authorizationUrl: https://shopify.com/authentication/67598516522/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/67598516522/oauth/token\n    pkce: S256\nscopes:\n  - name: openid\n    description: OpenID Connect — request an ID token identifying the signed-in customer.\n  - name: email\n    description: Release the customer's email address and email_verified claim.\n  - name: customer-account-api:full\n\
  \    description: >-\n      Full access to the Shopify Customer Account API for the signed-in customer of the\n      hearthnhome.com store.\n  - name: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-account MCP API for the signed-in customer — the authenticated\n      counterpart to the anonymous UCP commerce endpoint.\nscope_count: 4\ngranularity: coarse\ngranularity_note: >-\n  Two of the four scopes are `:full` grants. There is no read/write or per-resource split, so an agent\n  authorized for customer account data receives the whole account surface.\nevidence:\n  url: https://hearthnhome.com/.well-known/oauth-authorization-server\n  http_status: 200\n  probed: '2026-09-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hni/refs/heads/main/scopes/hni-scopes.yml
summary_line: 4 scopes · authorization_code
tags:
- Fortune 1000
- Manufacturing
- Office Furniture
- Workplace
- Building Products
- Hearth
- Retail
- E-Commerce
- Agentic Commerce
- MCP
token_bound: false
token_urls:
- https://shopify.com/authentication/67598516522/oauth/token
---
