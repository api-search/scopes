---
authorization_urls:
- https://shopify.com/authentication/53345157285/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Paperless Post Scopes
name_suffix: OAuth Scopes
note: Scopes are the `scopes_supported` array advertised by the authorization server that protects the Paperless Post Party Shop storefront. Paperless Post publishes no scope reference of its own; descriptions below state only what each scope literally names. The core www.paperlesspost.com product has no OAuth surface at all.
overview: 'Paperless Post publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paperless Post API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/53345157285/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paperless Post
provider_slug: paperless-post
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/53345157285/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/53345157285/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/paperless-post-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's account API surface.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated customer's account MCP API surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: paperless-post-scopes
source_filename: paperless-post-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://partyshop.paperlesspost.com/.well-known/openid-configuration\nnote: >-\n  Scopes are the `scopes_supported` array advertised by the authorization server\n  that protects the Paperless Post Party Shop storefront. Paperless Post\n  publishes no scope reference of its own; descriptions below state only what\n  each scope literally names. The core www.paperlesspost.com product has no\n  OAuth surface at all.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/paperless-post-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/53345157285/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/53345157285/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/paperless-post-openid-configuration.json]\n- scope:\
  \ email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/paperless-post-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's account API surface.\n  flows: [authorizationCode]\n  sources: [well-known/paperless-post-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated customer's account MCP API surface.\n  flows: [authorizationCode]\n  sources: [well-known/paperless-post-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://partyshop.paperlesspost.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperless-post/refs/heads/main/scopes/paperless-post-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Invitations
- Events
- Greeting Cards
- Stationery
- Consumer
- E-Commerce
- RSVP
- Design
token_urls:
- https://shopify.com/authentication/53345157285/oauth/token
---
