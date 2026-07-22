---
authorization_urls:
- https://shopify.com/authentication/3960733763/oauth/authorize
description: ''
docs: https://innovist.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Innovist Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Innovist publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Innovist API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/3960733763/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Innovist
provider_slug: innovist
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/3960733763/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/3960733763/oauth/token
  name: shopifyCustomerAccountOIDC
  source: well-known/innovist-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API used for agent-driven commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: innovist-scopes
source_filename: innovist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://innovist.com/.well-known/openid-configuration\ndocs: https://innovist.com/.well-known/oauth-authorization-server\nnotes: >-\n  OAuth/OIDC scopes captured verbatim from the store's live discovery documents\n  (scopes_supported). These are Shopify customer-account identity scopes, plus\n  the customer-account MCP API scope that backs agent-driven commerce.\nschemes:\n- name: shopifyCustomerAccountOIDC\n  source: well-known/innovist-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/3960733763/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/3960733763/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows:\n  - authorizationCode\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n-\
  \ scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows:\n  - authorizationCode\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API used for agent-driven commerce.\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovist/refs/heads/main/scopes/innovist-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Personal Care
- Skincare
- Haircare
- Suncare
- Direct to Consumer
- Ecommerce
- Shopify
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/3960733763/oauth/token
---
