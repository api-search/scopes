---
authorization_urls:
- https://us-account.soundboks.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Soundboks Scopes
name_suffix: OAuth Scopes
note: scopes_supported taken verbatim from the live OIDC discovery document on soundboks.com. These are Shopify Customer Accounts platform scopes, not Soundboks-authored scopes.
overview: 'Soundboks publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Soundboks API on a user''s behalf.


  Tokens are issued from https://us-account.soundboks.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Soundboks
provider_slug: soundboks
schemes:
- flows:
  - authorizationUrl: https://us-account.soundboks.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://us-account.soundboks.com/authentication/oauth/token
  name: oauth2
  source: well-known/soundboks-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the customer.
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
- description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: soundboks-scopes
source_filename: soundboks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://soundboks.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  scopes_supported taken verbatim from the live OIDC discovery document on\n  soundboks.com. These are Shopify Customer Accounts platform scopes, not\n  Soundboks-authored scopes.\nschemes:\n- name: oauth2\n  source: well-known/soundboks-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us-account.soundboks.com/authentication/oauth/authorize\n    tokenUrl: https://us-account.soundboks.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/soundboks-openid-configuration.json\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/soundboks-openid-configuration.json\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/soundboks-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/soundboks-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundboks/refs/heads/main/scopes/soundboks-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Electronics
- Audio
- Bluetooth Speakers
- Hardware
- E-commerce
- Shopify
- Direct-to-Consumer
token_urls:
- https://us-account.soundboks.com/authentication/oauth/token
---
