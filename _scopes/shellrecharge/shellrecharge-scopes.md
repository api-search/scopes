---
api_specs:
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Locations API
  slug: shellrecharge-public-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Charge Sessions API
  slug: shellrecharge-public-charge-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge OCPI API
  slug: shellrecharge-ocpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tariffs API
  slug: shellrecharge-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tokens API
  slug: shellrecharge-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.shell.com/docs/authentication-authorisation
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Shellrecharge Scopes
name_suffix: OAuth Scopes
note: Shell Developer APIs use the OAuth 2.0 client credentials grant with no published scopes; access is governed by partner credentials issued per app by the Shell API team (https://developer.shell.com/docs/authentication-authorisation).
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
  source: openapi/shellrecharge-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: shellrecharge-scopes
source_filename: shellrecharge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shellrecharge-openapi.yml\ndocs: https://developer.shell.com/docs/authentication-authorisation\nnote: Shell Developer APIs use the OAuth 2.0 client credentials grant with no published\n  scopes; access is governed by partner credentials issued per app by the Shell API\n  team (https://developer.shell.com/docs/authentication-authorisation).\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/shellrecharge-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the\n    Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret\n    pair is also required on functional requests.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/scopes/shellrecharge-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- EV Charging
- Electric Vehicles
- Mobility
- Charge Points
- OCPI
- Energy
token_urls:
- https://api.shell.com/v1/oauth/token
---
