---
authorization_urls: []
description: ''
docs: https://docs.shippingapi.pitneybowes.com/api/post-oauth-token.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Pitney Bowes Scopes
name_suffix: OAuth Scopes
note: Pitney Bowes Shipping APIs use the OAuth client_credentials grant with a Base64-encoded API key and secret, and do not publish user-selectable OAuth scopes; access is tied to the developer account credentials (https://docs.shippingapi.pitneybowes.com/api/post-oauth-token.html).
overview: 'Pitney Bowes uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://shipping-api.pitneybowes.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pitney Bowes
provider_slug: pitney-bowes
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://shipping-api.pitneybowes.com/oauth/token
  name: oauth2
  source: openapi/pitney-bowes-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: pitney-bowes-scopes
source_filename: pitney-bowes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pitney-bowes-openapi.yml\ndocs: https://docs.shippingapi.pitneybowes.com/api/post-oauth-token.html\nnote: Pitney Bowes Shipping APIs use the OAuth client_credentials grant with a Base64-encoded\n  API key and secret, and do not publish user-selectable OAuth scopes; access is tied to\n  the developer account credentials (https://docs.shippingapi.pitneybowes.com/api/post-oauth-token.html).\nschemes:\n- name: oauth2\n  source: openapi/pitney-bowes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shipping-api.pitneybowes.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/scopes/pitney-bowes-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Mailing
- Shipping
- Fortune 1000
token_urls:
- https://shipping-api.pitneybowes.com/oauth/token
---
