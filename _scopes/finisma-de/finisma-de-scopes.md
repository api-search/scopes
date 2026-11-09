---
api_specs:
- filename: finisma-de-konto-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Konto API
  slug: finisma-de-konto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-konto-api-openapi.yml
- filename: finisma-de-kontoausz-ge-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Kontoauszüge API
  slug: finisma-de-kontoausz-ge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-kontoausz-ge-api-openapi.yml
- filename: finisma-de-partner-checks-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Partner Checks API
  slug: finisma-de-partner-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-partner-checks-api-openapi.yml
- filename: finisma-de-rechnungen-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Rechnungen API
  slug: finisma-de-rechnungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-rechnungen-api-openapi.yml
- filename: finisma-de-selbstauskunft-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Selbstauskunft API
  slug: finisma-de-selbstauskunft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-selbstauskunft-api-openapi.yml
- filename: finisma-de-zahlungsverkehr-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Zahlungsverkehr API
  slug: finisma-de-zahlungsverkehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-zahlungsverkehr-api-openapi.yml
authorization_urls:
- https://finisma.de/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Finisma De Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paulibytes UG (haftungsbeschränkt) publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paulibytes UG (haftungsbeschränkt) API on a user''s behalf.


  Tokens are issued from https://finisma.de/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paulibytes UG (haftungsbeschränkt)
provider_slug: finisma-de
schemes:
- description: OAuth 2.1 mit PKCE (S256). Clients können sich per Dynamic Client Registration unter /api/oauth/register selbst anmelden.
  flows:
  - authorizationUrl: https://finisma.de/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://finisma.de/api/oauth/token
  name: oauth2
  source: openapi/finisma-de-openapi.json
scope_count: 2
scope_names:
- invoice:create
- invoice:verify
scopes:
- description: ZUGFeRD-Rechnungen erzeugen
  flows:
  - authorizationCode
  scope: invoice:create
- description: E-Rechnungen prüfen
  flows:
  - authorizationCode
  scope: invoice:verify
slug: finisma-de-scopes
source_filename: finisma-de-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/finisma-de-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/finisma-de-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://finisma.de/api/oauth/authorize\n    tokenUrl: https://finisma.de/api/oauth/token\n  description: OAuth 2.1 mit PKCE (S256). Clients können sich per Dynamic Client Registration\n    unter /api/oauth/register selbst anmelden.\nscopes:\n- scope: invoice:create\n  description: ZUGFeRD-Rechnungen erzeugen\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/finisma-de-openapi.json\n- scope: invoice:verify\n  description: E-Rechnungen prüfen\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/finisma-de-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/finisma-de/scopes/finisma-de-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- FinTech
- Invoice
- PDF
- ZUGFeRD
- API
token_bound: false
token_urls:
- https://finisma.de/api/oauth/token
---
