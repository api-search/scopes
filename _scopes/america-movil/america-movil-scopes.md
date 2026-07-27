---
api_specs:
- filename: america-movil-claro-sim-swap-openapi.json
  format: json
  label: Claro SIM Swap API
  slug: claro-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-claro-sim-swap-openapi.json
- filename: america-movil-claro-device-location-openapi.json
  format: json
  label: Claro Device Location API
  slug: claro-device-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-claro-device-location-openapi.json
- filename: america-movil-claro-device-location-verify-camara-openapi.yaml
  format: yaml
  label: Claro Device Location Verify API
  slug: claro-device-location-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-claro-device-location-verify-camara-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: America Movil Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'América Móvil publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the América Móvil API on a user''s behalf.


  Tokens are issued from /oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: América Móvil
provider_slug: america-movil
schemes:
- flows:
  - absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token
    declared_scopes: 0
    flow: clientCredentials
    tokenUrl: /oauth2/v1/token
  name: OAuth2
  source: openapi/america-movil-claro-sim-swap-openapi.json
- flows:
  - absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token
    declared_scopes: 0
    flow: clientCredentials
    tokenUrl: /oauth2/v1/token
  name: OAuth2
  source: openapi/america-movil-claro-device-location-openapi.json
scope_count: 2
scope_names:
- retrieve-sim-swap-date
- check-sim-swap
scopes:
- description: Read the timestamp of the most recent SIM pairing change for a line (operation retrieveSimSwapDate).
  flows:
  - clientCredentials
  scope: retrieve-sim-swap-date
- description: Ask whether a SIM swap occurred within a caller-supplied window (operation checkSimSwap).
  flows:
  - clientCredentials
  scope: check-sim-swap
slug: america-movil-scopes
source_filename: america-movil-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: >-\n  openapi/america-movil-claro-device-location-openapi.json,\n  openapi/america-movil-claro-sim-swap-openapi.json\ndocs: null\ndocs_note: >-\n  Claro Brasil publishes no scopes or permissions reference page. The marketplace\n  grants access per API through an approval workflow rather than through a scope\n  catalog, and both harvested specifications declare an EMPTY scopes map on the\n  clientCredentials flow while still requiring named scopes at the operation\n  level — so the only scope evidence is the operation security requirements\n  below.\nschemes:\n- name: OAuth2\n  source: openapi/america-movil-claro-sim-swap-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v1/token\n    absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token\n    declared_scopes: 0\n- name: OAuth2\n  source: openapi/america-movil-claro-device-location-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ /oauth2/v1/token\n    absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token\n    declared_scopes: 0\nscopes:\n- scope: retrieve-sim-swap-date\n  description: >-\n    Read the timestamp of the most recent SIM pairing change for a line\n    (operation retrieveSimSwapDate).\n  flows: [clientCredentials]\n  sources:\n  - openapi/america-movil-claro-sim-swap-openapi.json\n- scope: check-sim-swap\n  description: >-\n    Ask whether a SIM swap occurred within a caller-supplied window\n    (operation checkSimSwap).\n  flows: [clientCredentials]\n  sources:\n  - openapi/america-movil-claro-sim-swap-openapi.json\ngaps:\n- The flow-level scopes map is empty in both specs, so a client cannot request these scopes from metadata alone.\n- The LBS device-location operation declares OAuth2 with no scope requirement at all, alongside Basic, Bearer and X-API-Key alternatives.\n- >-\n  No CAMARA-standard scope (e.g. device-location-read) appears in any\n  Claro-published document — only in the upstream\
  \ CAMARA definition Claro links\n  from its Device Location Verify product page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/scopes/america-movil-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Telecommunications
- Mexico
- Latin America
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Device Location
- Broadband
- 5G
- Carrier
token_urls:
- /oauth2/v1/token
---
