---
api_specs:
- filename: select-medical-holdings-fhir-r4-openapi.yml
  format: yaml
  label: Select Medical FHIR R4 API
  slug: select-medical-holdings-fhir-r4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/openapi/select-medical-holdings-fhir-r4-openapi.yml
authorization_urls: []
description: ''
docs: https://fhir.epic.com/Documentation?docId=oauth2
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Select Medical Holdings Scopes
name_suffix: OAuth Scopes
note: 'scopes_supported is read verbatim from the server''s own SMART discovery document (HTTP 200, fetched 2026-08-28). IMPORTANT: this list is the set of NON-FHIR scopes the endpoint advertises. SMART resource scopes (patient/*.read, user/*.read and the v2 patient/Observation.rs form) are NOT enumerated in scopes_supported — Epic grants them per registered application — but the server does declare permission-patient, permission-user, permission-v1 and permission-v2 among its SMART capabilities, which is the machine-readable statement that those scope families are supported. They are recorded below as `enumerated: false` so nothing here asserts a scope string the provider did not publish.'
overview: 'Select Medical Holdings publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Select Medical Holdings API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Select Medical Holdings
provider_slug: select-medical-holdings
schemes:
- authorizationUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/authorize
  name: smartOnFhir
  standard: SMART App Launch
  tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token
scope_count: 5
scope_names:
- openid
- profile
- fhirUser
- launch
- epic.scanning.dmsusername
scopes:
- description: OpenID Connect authentication — returns an id_token identifying the end user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect profile claims for the authenticated user.
  flows:
  - authorizationCode
  scope: profile
- description: SMART scope returning a reference to the FHIR resource (Practitioner, Patient or RelatedPerson) representing the authorized user.
  flows:
  - authorizationCode
  scope: fhirUser
- description: SMART EHR-launch context scope — lets an app launched from inside Epic inherit the current patient and encounter context.
  flows:
  - authorizationCode
  scope: launch
- description: Epic-proprietary scope carrying the document-management-system scanning username. Vendor-specific, not part of the SMART specification.
  flows:
  - authorizationCode
  scope: epic.scanning.dmsusername
slug: select-medical-holdings-scopes
source_filename: select-medical-holdings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration\ndocs: https://fhir.epic.com/Documentation?docId=oauth2\nnote: >-\n  scopes_supported is read verbatim from the server's own SMART discovery document (HTTP 200,\n  fetched 2026-08-28). IMPORTANT: this list is the set of NON-FHIR scopes the endpoint advertises.\n  SMART resource scopes (patient/*.read, user/*.read and the v2 patient/Observation.rs form) are NOT\n  enumerated in scopes_supported — Epic grants them per registered application — but the server does\n  declare permission-patient, permission-user, permission-v1 and permission-v2 among its SMART\n  capabilities, which is the machine-readable statement that those scope families are supported.\n  They are recorded below as `enumerated: false` so nothing here asserts a scope string the provider\n  did not publish.\nschemes:\n  - name: smartOnFhir\n    authorizationUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/authorize\n\
  \    tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token\n    standard: SMART App Launch\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication — returns an id_token identifying the end user.\n    enumerated: true\n    flows: [authorizationCode]\n  - scope: profile\n    description: Standard OpenID Connect profile claims for the authenticated user.\n    enumerated: true\n    flows: [authorizationCode]\n  - scope: fhirUser\n    description: >-\n      SMART scope returning a reference to the FHIR resource (Practitioner, Patient or RelatedPerson)\n      representing the authorized user.\n    enumerated: true\n    flows: [authorizationCode]\n  - scope: launch\n    description: >-\n      SMART EHR-launch context scope — lets an app launched from inside Epic inherit the current\n      patient and encounter context.\n    enumerated: true\n    flows: [authorizationCode]\n  - scope: epic.scanning.dmsusername\n    description: >-\n      Epic-proprietary\
  \ scope carrying the document-management-system scanning username. Vendor-specific,\n      not part of the SMART specification.\n    enumerated: true\n    vendor_specific: true\n    flows: [authorizationCode]\nscope_families_declared:\n  - family: patient/*\n    enumerated: false\n    evidence: SMART capability \"permission-patient\" declared in smart-configuration\n    note: Patient-context resource scopes, granted per registered app rather than advertised.\n  - family: user/*\n    enumerated: false\n    evidence: SMART capability \"permission-user\" declared in smart-configuration\n    note: User-context resource scopes, granted per registered app.\n  - family: SMART v1 scope syntax\n    enumerated: false\n    evidence: SMART capability \"permission-v1\" declared in smart-configuration\n  - family: SMART v2 scope syntax\n    enumerated: false\n    evidence: SMART capability \"permission-v2\" declared in smart-configuration\n    note: v2 granular scopes (e.g. patient/Observation.rs) are\
  \ supported.\n  - family: offline_access\n    enumerated: false\n    evidence: SMART capability \"permission-offline\" declared; refresh_token grant type supported\nx-evidence:\n  - url: https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration\n    http_status: 200\n    fetched: '2026-08-28'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/scopes/select-medical-holdings-scopes.yml
summary_line: 5 scopes
tags:
- Healthcare
- Hospitals
- Rehabilitation
- Patient Access
- FHIR
- Interoperability
- Electronic Health Records
- Fortune 1000
token_urls: []
---
