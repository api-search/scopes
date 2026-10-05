---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorization_code (PKCE, S256)
- refresh_token
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: True And Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'True & Co publishes 4 OAuth 2.0 scopes via the authorization_code (PKCE, S256), refresh_token, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the True & Co API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: True & Co
provider_slug: true-and-co
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the customer.
  flows: []
  scope: openid
- description: Access to the customer's verified email address claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven access to the buyer's account.
  flows: []
  scope: customer-account-mcp-api:full
slug: true-and-co-scopes
source_filename: true-and-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: 2026-07-21\nmethod: searched\nsource: >-\n  https://trueandco.com/.well-known/openid-configuration (scopes_supported),\n  fetched live 2026-07-21\nprovider: Shopify Customer Account (OAuth 2.0 / OIDC)\nissuer: https://shopify.com/authentication/86218834196\ndocs: https://shopify.dev/docs/api/customer\nflows:\n- authorization_code (PKCE, S256)\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\nscopes:\n- name: openid\n  description: OpenID Connect authentication; issues an ID token for the customer.\n- name: email\n  description: Access to the customer's verified email address claim.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in buyer.\n- name: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API for agent-driven access to the buyer's account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-and-co/refs/heads/main/scopes/true-and-co-scopes.yml
summary_line: 4 scopes · authorization_code (PKCE, S256)/refresh_token/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Apparel
- Intimates
- Agentic Commerce
- Shopify
- MCP
token_bound: false
token_urls: []
---
