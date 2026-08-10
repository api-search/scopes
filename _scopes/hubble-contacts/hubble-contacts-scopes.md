---
authorization_urls:
- https://shopify.com/authentication/15165228/oauth/authorize
description: ''
docs: https://account.hubblecontacts.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hubble Contacts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hubble Contacts publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hubble Contacts API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/15165228/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hubble Contacts
provider_slug: hubble-contacts
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/15165228/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/15165228/oauth/token
  issuer: https://shopify.com/authentication/15165228
  name: shopify-customer-accounts
  source: well-known/hubble-contacts-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's account API — orders, subscriptions, addresses and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer account surface over MCP, for agents acting on the authenticated customer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: hubble-contacts-scopes
source_filename: hubble-contacts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://account.hubblecontacts.com/.well-known/openid-configuration\ndocs: https://account.hubblecontacts.com/.well-known/oauth-authorization-server\nnotes: >-\n  Scopes are read verbatim from the scopes_supported array of the OAuth/OIDC\n  discovery documents Hubble's storefront host serves. There is no OpenAPI with\n  oauth2 securitySchemes to derive from, and Hubble publishes no scope reference page\n  of its own — the authorization server is the Shopify customer accounts issuer bound\n  to Hubble's shop id. Descriptions below are the standard meanings of these scopes;\n  no scope is listed that the discovery document does not name.\nschemes:\n- name: shopify-customer-accounts\n  issuer: https://shopify.com/authentication/15165228\n  source: well-known/hubble-contacts-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/15165228/oauth/authorize\n    tokenUrl:\
  \ https://shopify.com/authentication/15165228/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/hubble-contacts-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/hubble-contacts-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: Full access to the authenticated customer's account API — orders, subscriptions, addresses and profile.\n  flows: [authorizationCode]\n  sources: [well-known/hubble-contacts-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the customer account surface over MCP, for agents acting on the authenticated customer's behalf.\n  flows: [authorizationCode]\n  sources: [well-known/hubble-contacts-openid-configuration.json]\n\
  x-evidence:\n  fetched: '2026-08-04'\n  url: https://account.hubblecontacts.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-contacts/refs/heads/main/scopes/hubble-contacts-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Health
- Vision Care
- Contact Lenses
- Subscriptions
- Agentic Commerce
- Model Context Protocol
- Shopify
- GraphQL
token_urls:
- https://shopify.com/authentication/15165228/oauth/token
---
