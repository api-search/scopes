---
authorization_urls: []
description: ''
docs: https://developer.ups.com/api/reference/oauth/client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ups Scopes
name_suffix: OAuth Scopes
note: UPS OAuth 2.0 does not publish named scopes — the client credentials token request takes no scope parameter and the authorization-code spec leaves scope as an undocumented free-form string, with API permissions instead granted by adding API products to an application in the UPS Developer Portal (https://developer.ups.com/api/reference/oauth/client-credentials).
overview: 'UPS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://onlinetools.ups.com/api/security/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UPS
provider_slug: ups
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  source: openapi/ups-shipping-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ups-scopes
source_filename: ups-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ups-shipping-openapi.yml\ndocs: https://developer.ups.com/api/reference/oauth/client-credentials\nnote: UPS OAuth 2.0 does not publish named scopes — the client credentials token\n  request takes no scope parameter and the authorization-code spec leaves scope as\n  an undocumented free-form string, with API permissions instead granted by adding\n  API products to an application in the UPS Developer Portal (https://developer.ups.com/api/reference/oauth/client-credentials).\nschemes:\n- name: OAuth2\n  source: openapi/ups-shipping-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/scopes/ups-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Logistics
- Shipping
- Fortune 500
- Supply Chain
token_urls:
- https://onlinetools.ups.com/api/security/v1/oauth/token
---
