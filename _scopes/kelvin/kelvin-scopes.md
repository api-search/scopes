---
api_specs:
- filename: kelvin-api-openapi.yml
  format: yaml
  label: kelvin API
  slug: kelvin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/openapi/kelvin-api-openapi.yml
authorization_urls: []
description: ''
docs: https://app.go-kelvin.com/api/docs
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Kelvin Scopes
name_suffix: OAuth Scopes
note: 'kelvin does not run OAuth 2.0 — there is no authorization server, no securityScheme of type oauth2 and no scopes map in either spec, so derive-oauth-scopes.py finds nothing. Authorization is nevertheless scope-based: the team API key carries scopes, and the specification''s 403 descriptions name one of them explicitly and refer to others generically ("Scope manquant"). Only the scope kelvin actually names is recorded below; the rest are recorded as an unenumerated set rather than guessed.'
overview: 'Kelvin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kelvin
provider_slug: kelvin
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kelvin-scopes
source_filename: kelvin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: >-\n  openapi/kelvin-api-openapi.yml — 403 response descriptions on the kelvin API v3\n  specification harvested from https://app.go-kelvin.com/api/docs\ndocs: https://app.go-kelvin.com/api/docs\napi: kelvin API\nmodel: api-key-scopes\noauth2: false\nnote: >-\n  kelvin does not run OAuth 2.0 — there is no authorization server, no securityScheme\n  of type oauth2 and no scopes map in either spec, so derive-oauth-scopes.py finds\n  nothing. Authorization is nevertheless scope-based: the team API key carries scopes,\n  and the specification's 403 descriptions name one of them explicitly and refer to\n  others generically (\"Scope manquant\"). Only the scope kelvin actually names is\n  recorded below; the rest are recorded as an unenumerated set rather than guessed.\nscopes:\n- name: catalog:read\n  documented: true\n  source: >-\n    403 description \"Forbidden - scope catalog:read manquant\" on the three\n    /api/v3/catalog/enabled/*\
  \ operations\n  grants:\n  - GET /api/v3/catalog/enabled/gestures\n  - GET /api/v3/catalog/enabled/references\n  - GET /api/v3/catalog/enabled/services\n  description: >-\n    Read the team's enabled catalogue of work gestures, services and pricing\n    references.\nunenumerated_scopes:\n  count: unknown\n  evidence:\n  - description: 'Forbidden - Scope manquant ou document désactivé pour l''équipe.'\n    operations:\n    - POST /api/v3/simulations/{simulation_id}/documents/report\n    - POST /api/v3/simulations/{simulation_id}/documents/contribution-framework\n    - POST /api/v3/simulations/{simulation_id}/documents/dimensioning-note\n    - POST /api/v3/simulations/{simulation_id}/documents/sworn-statement\n  - description: 'Forbidden - Scope manquant ou devis désactivés pour l''équipe.'\n    operations:\n    - POST /api/v3/simulations/{simulation_id}/documents/commercial-offer\n  note: >-\n    Document generation and quote generation are gated by scopes whose names kelvin\n    does not\
  \ publish, and the same 403 also fires when the feature is merely disabled\n    for the team. A caller cannot determine from the response which of the two applies,\n    and cannot request a scope by name because no name exists in the documentation.\nentitlement_tiers:\n  note: >-\n    The specification's tags double as commercial offers — \"Endpoints disponibles dans\n    l'offre Simulateur\", \"Endpoints disponibles dans l'offre Qualification\", plus a\n    Documents group. Access therefore depends on the purchased offer as well as the\n    scope on the key. See plans/kelvin-plans-pricing.yml.\n  tiers:\n  - name: Simulateur\n    operations: 6\n  - name: Qualification\n    operations: 12\n  - name: Documents\n    operations: 7\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/scopes/kelvin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Energy
- Energy Efficiency
- Home Renovation
- Construction
- Artificial Intelligence
- Lead Generation
- Sales Enablement
- France
- Sustainability
token_urls: []
---
