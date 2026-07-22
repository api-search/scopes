---
authorization_urls:
- https://shopify.com/authentication/63049990366/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Uscoop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'uScoop publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the uScoop API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/63049990366/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: uScoop
provider_slug: uscoop
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/63049990366/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/63049990366/oauth/token
  name: shopify-customer-accounts-oauth2
  source: well-known/uscoop-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (standard OIDC scope)
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address (standard OIDC scope)
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for this store
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify customer-account MCP API for this store
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: uscoop-scopes
source_filename: uscoop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tnuck.com/.well-known/openid-configuration\nschemes:\n- name: shopify-customer-accounts-oauth2\n  source: well-known/uscoop-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/63049990366/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/63049990366/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (standard OIDC scope)\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/uscoop-openid-configuration.json\n- scope: email\n  description: Access to the customer's email address (standard OIDC scope)\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/uscoop-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for this store\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/uscoop-openid-configuration.json\n\
  - scope: customer-account-mcp-api:full\n  description: Full access to the Shopify customer-account MCP API for this store\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/uscoop-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uscoop/refs/heads/main/scopes/uscoop-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- Fashion
- eCommerce
- Agentic Commerce
- Shopping
token_urls:
- https://shopify.com/authentication/63049990366/oauth/token
---
