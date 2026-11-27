---
api_specs:
- filename: brreg-no-enheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Enheter API
  slug: brreg-no-enheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-enheter-api-openapi.yml
- filename: brreg-no-frivillighetsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Frivillighetsregisteret API
  slug: brreg-no-frivillighetsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-frivillighetsregisteret-api-openapi.yml
- filename: brreg-no-generelt-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Generelt API
  slug: brreg-no-generelt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-generelt-api-openapi.yml
- filename: brreg-no-kommuner-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kommuner API
  slug: brreg-no-kommuner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kommuner-api-openapi.yml
- filename: brreg-no-kopi-av-rsregnskap-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kopi av årsregnskap API
  slug: brreg-no-kopi-av-rsregnskap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kopi-av-rsregnskap-api-openapi.yml
- filename: brreg-no-matrikkelenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Matrikkelenheter API
  slug: brreg-no-matrikkelenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-matrikkelenheter-api-openapi.yml
- filename: brreg-no-mellombalanse-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Mellombalanse API
  slug: brreg-no-mellombalanse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-mellombalanse-api-openapi.yml
- filename: brreg-no-oppdateringer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Oppdateringer API
  slug: brreg-no-oppdateringer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-oppdateringer-api-openapi.yml
- filename: brreg-no-organisasjonsformer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Organisasjonsformer API
  slug: brreg-no-organisasjonsformer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-organisasjonsformer-api-openapi.yml
- filename: brreg-no-partiregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Partiregisteret API
  slug: brreg-no-partiregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-partiregisteret-api-openapi.yml
- filename: brreg-no-regnskapsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Regnskapsregisteret API
  slug: brreg-no-regnskapsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-regnskapsregisteret-api-openapi.yml
- filename: brreg-no-roller-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Roller API
  slug: brreg-no-roller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-roller-api-openapi.yml
- filename: brreg-no-statistikk-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Statistikk API
  slug: brreg-no-statistikk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-statistikk-api-openapi.yml
- filename: brreg-no-underenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Underenheter API
  slug: brreg-no-underenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-underenheter-api-openapi.yml
authorization_urls: []
description: ''
docs: https://data.brreg.no/enhetsregisteret/api/docs/index.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Brønnøysundregistrene Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brønnøysundregistrene publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brønnøysundregistrene API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brønnøysundregistrene
provider_slug: brreg-no
schemes: []
scope_count: 1
scope_names:
- brreg:data:enhetsregisteret:roller:person:oppslag:fnr
scopes:
- description: Look up all roles a person holds in business entities by national identity number (fødselsnummer) on the autorisert-api.
  flows: []
  scope: brreg:data:enhetsregisteret:roller:person:oppslag:fnr
slug: brreg-no-scopes
source_filename: brreg-no-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Brønnøysundregistrene OAuth scopes\ngenerated: '2026-11-10'\nmethod: searched\nsource: https://data.brreg.no/enhetsregisteret/api/docs/index.html#section/Endringslogg\ndocs: https://data.brreg.no/enhetsregisteret/api/docs/index.html\nauthorization_server: Maskinporten (Norwegian Digitalisation Agency)\nscopes:\n- name: brreg:data:enhetsregisteret:roller:person:oppslag:fnr\n  description: Look up all roles a person holds in business entities by national identity number (fødselsnummer) on the autorisert-api.\n"
source_yaml_url: https://artifacts.apis.io/brreg-no/scopes/brreg-no-scopes.yml
summary_line: 1 scope
tags:
- Government
- Business Registry
- Open Data
- Norway
- Company Data
- Public Sector
- Financial Statements
token_bound: false
token_urls: []
---
