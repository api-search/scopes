---
api_specs:
- filename: la-poste-groupe-suivi-openapi.json
  format: json
  label: La Poste Suivi v2
  slug: la-poste-suivi-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-suivi-openapi.json
- filename: la-poste-groupe-digiposte-openapi.json
  format: json
  label: Digiposte v3
  slug: digiposte-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-digiposte-openapi.json
- filename: la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
  format: json
  label: Lettre recommandee en ligne v1
  slug: lettre-recommandee-en-ligne-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
- filename: la-poste-groupe-open-data-openapi.json
  format: json
  label: La Poste Open Data v1
  slug: la-poste-open-data-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-open-data-openapi.json
authorization_urls:
- /
- https://test.com
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: La Poste Groupe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'La Poste Groupe uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: La Poste Groupe
provider_slug: la-poste-groupe
schemes:
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/la-poste-groupe-digiposte-openapi.json
- flows:
  - authorizationUrl: https://test.com
    flow: implicit
  name: default
  source: openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: la-poste-groupe-scopes
source_filename: la-poste-groupe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/la-poste-groupe-digiposte-openapi.json, openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/la-poste-groupe-digiposte-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: default\n  source: openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://test.com\nscopes: []\nscope_count: 0\nfinding: >-\n  Both oauth2 declarations in this estate carry an EMPTY scopes map, and no scope or\n  permission reference page exists on developer.laposte.fr,\n  faq.developer.laposte.fr or documentation-okapi.laposte.fr (searched 2026-09-02).\n  Digiposte v3 uses client_credentials with no scope narrowing - a partner token is\n  all-or-nothing across memberships, certified deposit, organisation safes and\n  sharing. Lettre recommandee en ligne's oauth2 block is a\
  \ springdoc placeholder\n  pointed at https://test.com and is not a real authorization surface.\n  Authorisation on the rest of the estate is not OAuth at all: it is a per-plan\n  X-Okapi-Key, where the PLAN (not a scope) decides which routes and methods the\n  key may call - the portal exposes that as filteredRoutes / filteredMethods /\n  filteredResourcesCount on each plan.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/scopes/la-poste-groupe-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Logistics
- Shipping
- Package Tracking
- Postal
- Addresses
- Geocoding
- Open Data
- Document Management
- Identity
- Government
- France
token_urls:
- /
---
