---
api_specs:
- filename: shellrecharge-locations-api-openapi.yml
  format: yaml
  label: ShellRecharge Locations API
  slug: shellrecharge-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-locations-api-openapi.yml
- filename: shellrecharge-sessions-api-openapi.yml
  format: yaml
  label: ShellRecharge Sessions API
  slug: shellrecharge-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-sessions-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Shellrecharge Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'ShellRecharge uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.shell.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ShellRecharge
provider_slug: shellrecharge
schemes:
- description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret pair is also required on functional requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.shell.com/v1/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/shellrecharge-locations-api-openapi.yml
- description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret pair is also required on functional requests.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.shell.com/v1/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/shellrecharge-sessions-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: shellrecharge-scopes
source_filename: shellrecharge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/shellrecharge-locations-api-openapi.yml, openapi/shellrecharge-sessions-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/shellrecharge-locations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the\n    Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret\n    pair is also required on functional requests.\n- name: OAuth2ClientCredentials\n  source: openapi/shellrecharge-sessions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the\n    Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret\n    pair is also required on\
  \ functional requests.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/scopes/shellrecharge-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- EV Charging
- Electric Vehicles
- Mobility
- OCPI
- Energy
token_bound: false
token_urls:
- https://api.shell.com/v1/oauth/token
---
