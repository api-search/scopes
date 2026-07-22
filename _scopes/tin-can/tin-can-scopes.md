---
authorization_urls:
- https://manage.tincan.kids/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tin Can Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tin Can publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tin Can API on a user''s behalf.


  Tokens are issued from https://manage.tincan.kids/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tin Can
provider_slug: tin-can
schemes:
- flows:
  - authorizationUrl: https://manage.tincan.kids/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://manage.tincan.kids/authentication/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://shopify.com/authentication/89002967405
  name: Shopify Customer Accounts (OIDC)
  source: well-known/tin-can-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify customer-account MCP API surface for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: tin-can-scopes
source_filename: tin-can-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/tin-can-openid-configuration.json (fetched live from\n  https://tincan.kids/.well-known/openid-configuration, 2026-07-21)\ndocs: null\nnotes: >-\n  OAuth surface is the Shopify Customer Accounts authorization server published\n  on the provider's own domain. No first-party Tin Can scope documentation\n  exists; scopes below are exactly the scopes_supported advertised in the OIDC\n  discovery document.\nschemes:\n- name: Shopify Customer Accounts (OIDC)\n  source: well-known/tin-can-openid-configuration.json\n  issuer: https://shopify.com/authentication/89002967405\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://manage.tincan.kids/authentication/oauth/authorize\n    tokenUrl: https://manage.tincan.kids/authentication/oauth/token\n    pkce: S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\nscopes:\n- scope: openid\n  description:\
  \ OpenID Connect authentication.\n  flows: [authorizationCode]\n  sources: [well-known/tin-can-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/tin-can-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the\n    authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/tin-can-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify customer-account MCP API surface for\n    the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/tin-can-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tin-can/refs/heads/main/scopes/tin-can-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Hardware
- Telecommunications
- Voice
- Kids
- Phones
token_urls:
- https://manage.tincan.kids/authentication/oauth/token
---
