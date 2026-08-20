---
api_specs:
- filename: uc-davis-aggie-experts-api-openapi.yml
  format: yaml
  label: Aggie Experts API
  slug: aggie-experts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-aggie-experts-api-openapi.yml
- filename: uc-davis-dams-api-openapi.yml
  format: yaml
  label: DAMS API — UC Davis Library Digital Collections
  slug: dams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-dams-api-openapi.yml
- filename: uc-davis-access-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Access API
  slug: uc-davis-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-access-api-openapi.yml
- filename: uc-davis-documents-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Documents API
  slug: uc-davis-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-documents-api-openapi.yml
- filename: uc-davis-equipment-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Equipment API
  slug: uc-davis-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-equipment-api-openapi.yml
- filename: uc-davis-keys-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Keys API
  slug: uc-davis-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keys-api-openapi.yml
- filename: uc-davis-keyserials-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — KeySerials API
  slug: uc-davis-keyserials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keyserials-api-openapi.yml
- filename: uc-davis-people-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — People API
  slug: uc-davis-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-people-api-openapi.yml
- filename: uc-davis-peopleadmin-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — PeopleAdmin API
  slug: uc-davis-peopleadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-peopleadmin-api-openapi.yml
- filename: uc-davis-spaces-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Spaces API
  slug: uc-davis-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-spaces-api-openapi.yml
- filename: uc-davis-workstations-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Workstations API
  slug: uc-davis-workstations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-workstations-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Uc Davis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of California, Davis uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of California, Davis
provider_slug: uc-davis
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: uc-davis-scopes
source_filename: uc-davis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# generated: 2026-08-19 | method: derived (PEAKS) + probed (SMART configuration)\n---\nname: University of California, Davis — authorization scopes\nslug: uc-davis\ngenerated: '2026-08-19'\nmethod: derived\nsource: Derived from security[] in openapi/_original/uc-davis-peaks.yaml, and probed from the UC Davis\n  Health SMART configuration.\napis:\n- api: PEAKS API\n  operator: institution\n  scheme: ApiKey (X-Auth-Token header)\n  method: derived\n  source: openapi/_original/uc-davis-peaks.yaml security[] entries\n  scopes:\n  - scheme: ApiKey\n    scope: AccessMasterAccess\n  - scheme: ApiKey\n    scope: AnyRole\n  - scheme: ApiKey\n    scope: DocumentMasterAccess\n  - scheme: ApiKey\n    scope: EquipMasterAccess\n  - scheme: ApiKey\n    scope: KeyMasterAccess\n  - scheme: ApiKey\n    scope: PersonManagerAccess\n  - scheme: ApiKey\n    scope: SpaceMasterAccess\n- api: UC Davis Health FHIR R4\n  operator: institution\n  contract_author: Epic Systems\n  scheme: OAuth 2.0 / SMART\
  \ on FHIR\n  method: probed\n  source: https://emrrp.ucdmc.ucdavis.edu/FHIR/api/FHIR/R4/.well-known/smart-configuration\n  authorization_endpoint: https://emrrp.ucdmc.ucdavis.edu/FHIR/oauth2/authorize\n  token_endpoint: https://emrrp.ucdmc.ucdavis.edu/FHIR/oauth2/token\n  scopes:\n  - scope: epic.scanning.dmsusername\n    source: smart-configuration scopes_supported\n  - scope: fhirUser\n    source: smart-configuration scopes_supported\n  - scope: launch\n    source: smart-configuration scopes_supported\n  - scope: openid\n    source: smart-configuration scopes_supported\n  - scope: profile\n    source: smart-configuration scopes_supported\n- api: Aggie Experts API\n  operator: institution\n  scheme: none\n  method: probed\n  source: https://experts.ucdavis.edu/api/\n  detail: The contract declares no securitySchemes and read operations answer anonymously (verified live).\n    The /api/miv/* operations describe an authenticated MIV user but no scheme is declared for them —\n    an undocumented\
  \ auth boundary.\n  scopes: []\n- api: DAMS API\n  operator: institution\n  scheme: none-declared\n  method: probed\n  source: https://digital.ucdavis.edu/api/\n  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/scopes/uc-davis-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Research
- Research Data
- Identity Federation
- Digital Collections
- Library
- Health
- Open-Source
token_urls: []
---
