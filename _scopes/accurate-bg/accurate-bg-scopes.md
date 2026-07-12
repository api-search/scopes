---
authorization_urls: []
description: ''
docs: https://accurate.readme.io/reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Accurate Bg Scopes
name_suffix: OAuth Scopes
note: Accurate's API authenticates via an OAuth 2.0 client-credentials exchange of a ClientID/ClientSecret pair from the developer portal, and no OAuth scopes are documented anywhere in the API reference or developer portal (https://accurate.readme.io/reference/authentication).
overview: 'Accurate Background uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.accuratebackground.com/v3/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accurate Background
provider_slug: accurate-bg
schemes:
- description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that authorizes subsequent requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.accuratebackground.com/v3/oauth/token
  name: oauth2ClientCredentials
  source: openapi/accurate-bg-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: accurate-bg-scopes
source_filename: accurate-bg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accurate-bg-openapi.yml\ndocs: https://accurate.readme.io/reference/authentication\nnote: Accurate's API authenticates via an OAuth 2.0 client-credentials exchange of\n  a ClientID/ClientSecret pair from the developer portal, and no OAuth scopes are\n  documented anywhere in the API reference or developer portal\n  (https://accurate.readme.io/reference/authentication).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/accurate-bg-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.accuratebackground.com/v3/oauth/token\n  description: Accurate API credentials are a ClientID / ClientSecret pair obtained from the\n    Accurate developer portal. Credentials are exchanged (HTTP Basic) for an access token that\n    authorizes subsequent requests.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurate-bg/refs/heads/main/scopes/accurate-bg-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Background Checks
- Employment Screening
- Identity Verification
- Compliance
- HR Tech
- Screening
token_urls:
- https://api.accuratebackground.com/v3/oauth/token
---
