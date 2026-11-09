---
api_specs:
- filename: woz-api-nl-account-api-openapi.yml
  format: yaml
  label: woz-api-nl Account API
  slug: woz-api-nl-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-account-api-openapi.yml
- filename: woz-api-nl-adressen-api-openapi.yml
  format: yaml
  label: woz-api-nl Adressen API
  slug: woz-api-nl-adressen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-adressen-api-openapi.yml
- filename: woz-api-nl-lijst-api-openapi.yml
  format: yaml
  label: woz-api-nl Lijst API
  slug: woz-api-nl-lijst-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-lijst-api-openapi.yml
- filename: woz-api-nl-proef-api-openapi.yml
  format: yaml
  label: woz-api-nl Proef API
  slug: woz-api-nl-proef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-proef-api-openapi.yml
authorization_urls:
- https://woz-api.nl/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Woz Api Nl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'woz-api-nl publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the woz-api-nl API on a user''s behalf.


  Tokens are issued from https://woz-api.nl/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: woz-api-nl
provider_slug: woz-api-nl
schemes:
- description: 'OAuth-koppeling voor softwareleveranciers: authorization code met PKCE. Je klant koppelt zijn eigen Wozapi-account; credits gaan van diens saldo af.'
  flows:
  - authorizationUrl: https://woz-api.nl/connect/authorize
    flow: authorizationCode
    tokenUrl: https://woz-api.nl/connect/token
  name: OAuth2
  source: openapi/woz-api-nl-openapi.json
scope_count: 2
scope_names:
- account.saldo
- woz.lookup
scopes:
- description: Creditsaldo van de gekoppelde klant lezen
  flows:
  - authorizationCode
  scope: account.saldo
- description: WOZ-gegevens opvragen op de credits van de gekoppelde klant
  flows:
  - authorizationCode
  scope: woz.lookup
slug: woz-api-nl-scopes
source_filename: woz-api-nl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/woz-api-nl-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/woz-api-nl-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://woz-api.nl/connect/authorize\n    tokenUrl: https://woz-api.nl/connect/token\n  description: 'OAuth-koppeling voor softwareleveranciers: authorization code met PKCE. Je klant\n    koppelt zijn eigen Wozapi-account; credits gaan van diens saldo af.'\nscopes:\n- scope: account.saldo\n  description: Creditsaldo van de gekoppelde klant lezen\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/woz-api-nl-openapi.json\n- scope: woz.lookup\n  description: WOZ-gegevens opvragen op de credits van de gekoppelde klant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/woz-api-nl-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/woz-api-nl/scopes/woz-api-nl-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Real Estate
- Netherlands
- Property Valuation
- WOZ
token_bound: false
token_urls:
- https://woz-api.nl/connect/token
---
