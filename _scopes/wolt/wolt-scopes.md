---
authorization_urls: []
description: ''
docs: https://developer.wolt.com/docs/authentication20
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wolt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wolt publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wolt API on a user''s behalf.


  Tokens are issued from https://integrations-authentication-service.wolt.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wolt
provider_slug: wolt
schemes:
- flows:
  - flow: authorizationCode
    tokenUrl: https://integrations-authentication-service.wolt.com/oauth2/token
  name: OAuth2
  source: https://developer.wolt.com/docs/authentication20
scope_count: 1
scope_names:
- offline
scopes:
- description: Grants the offline access needed to obtain new access and refresh tokens (issues a refresh token alongside the access token).
  flows:
  - authorizationCode
  scope: offline
slug: wolt-scopes
source_filename: wolt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.wolt.com/docs/authentication20\ndocs: https://developer.wolt.com/docs/authentication20\nschemes:\n- name: OAuth2\n  source: https://developer.wolt.com/docs/authentication20\n  flows:\n  - flow: authorizationCode\n    tokenUrl: https://integrations-authentication-service.wolt.com/oauth2/token\nscopes:\n- scope: offline\n  description: >-\n    Grants the offline access needed to obtain new access and refresh tokens\n    (issues a refresh token alongside the access token).\n  flows: [authorizationCode]\n  sources: [https://developer.wolt.com/docs/authentication20]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolt/refs/heads/main/scopes/wolt-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Marketplace
- Food Delivery
- Last Mile Delivery
- Logistics
- Webhooks
- OAuth
- Point of Sale
token_urls:
- https://integrations-authentication-service.wolt.com/oauth2/token
---
