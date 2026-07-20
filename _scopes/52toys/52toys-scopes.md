---
authorization_urls: []
description: ''
docs: https://hi52toys.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: 52Toys Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Shopify customer-account authorization server backing the 52TOYS storefront and its UCP agentic-commerce MCP endpoint. Captured verbatim from scopes_supported in the live discovery document.
overview: '52TOYS publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the 52TOYS API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 52TOYS
provider_slug: 52toys
schemes:
- authorizationUrl: https://account.hi52toys.com/authentication/oauth/authorize
  issuer: https://shopify.com/authentication/77378748731
  name: shopify-customer-account-oidc
  tokenUrl: https://account.hi52toys.com/authentication/oauth/token
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the customer.
  flows: []
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on the shopper's behalf.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API for agent-driven commerce actions.
  flows: []
  scope: customer-account-mcp-api:full
slug: 52toys-scopes
source_filename: 52toys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://hi52toys.com/.well-known/openid-configuration\ndocs: https://hi52toys.com/.well-known/oauth-authorization-server\nnote: >-\n  OAuth/OIDC scopes advertised by the Shopify customer-account authorization\n  server backing the 52TOYS storefront and its UCP agentic-commerce MCP endpoint.\n  Captured verbatim from scopes_supported in the live discovery document.\nschemes:\n- name: shopify-customer-account-oidc\n  issuer: https://shopify.com/authentication/77378748731\n  authorizationUrl: https://account.hi52toys.com/authentication/oauth/authorize\n  tokenUrl: https://account.hi52toys.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  sources: [well-known/52toys-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  sources: [well-known/52toys-openid-configuration.json]\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on the shopper's behalf.\n  sources: [well-known/52toys-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API for agent-driven commerce actions.\n  sources: [well-known/52toys-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/52toys/refs/heads/main/scopes/52toys-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Consumer
- Collectibles
- Toys
- Retail
- Ecommerce
- Shopify
- Agentic Commerce
token_urls: []
---
