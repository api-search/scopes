---
authorization_urls:
- https://account.keyboard.io/authentication/oauth/authorize
description: ''
docs: https://keyboard.io/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Keyboardio Scopes
name_suffix: OAuth Scopes
note: OAuth scopes advertised by the Shopify Customer Accounts OpenID Connect discovery document served on keyboard.io. These are Shopify Customer Account API scopes, not scopes on a first-party Keyboardio API.
overview: 'Keyboardio publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Keyboardio API on a user''s behalf.


  Tokens are issued from https://account.keyboard.io/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keyboardio
provider_slug: keyboardio
schemes:
- flows:
  - authorizationUrl: https://account.keyboard.io/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.keyboard.io/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/keyboardio-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: keyboardio-scopes
source_filename: keyboardio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://keyboard.io/.well-known/openid-configuration\ndocs: https://keyboard.io/.well-known/openid-configuration\nnote: >-\n  OAuth scopes advertised by the Shopify Customer Accounts OpenID Connect\n  discovery document served on keyboard.io. These are Shopify Customer\n  Account API scopes, not scopes on a first-party Keyboardio API.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/keyboardio-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.keyboard.io/authentication/oauth/authorize\n    tokenUrl: https://account.keyboard.io/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/keyboardio-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/keyboardio-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/keyboardio-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/keyboardio-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyboardio/refs/heads/main/scopes/keyboardio-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Mechanical Keyboards
- Hardware
- Ergonomics
- Open Source
- Firmware
- Keyboards
- E-commerce
token_urls:
- https://account.keyboard.io/authentication/oauth/token
---
