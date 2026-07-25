---
authorization_urls:
- https://auth.1up.health/oauth2/authorize/system
description: ''
docs: https://docs.1up.health/docs/get-started/o-auth
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: 1Uphealth Scopes
name_suffix: OAuth Scopes
note: ''
overview: '1upHealth publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1upHealth API on a user''s behalf.


  Tokens are issued from https://auth.1up.health/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1upHealth
provider_slug: 1uphealth
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.1up.health/oauth2/token
  - authorizationUrl: https://auth.1up.health/oauth2/authorize/system
    flow: authorizationCode
    tokenUrl: https://auth.1up.health/oauth2/token
  name: SMARTonFHIR
  source: fhir/1uphealth-fhir-r4-capabilitystatement.json
scope_count: 1
scope_names:
- bulk-data|user/*.rs
scopes:
- description: Documented Bulk Data (Flat FHIR) export scope granting read/search across all resource types for the authorized user context. Verbatim from the OAuth docs.
  flows:
  - clientCredentials
  scope: bulk-data|user/*.rs
slug: 1uphealth-scopes
source_filename: 1uphealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: >-\n  fhir/1uphealth-fhir-r4-capabilitystatement.json (SMART-on-FHIR) +\n  https://docs.1up.health/docs/get-started/o-auth\ndocs: https://docs.1up.health/docs/get-started/o-auth\nmodel: SMART-on-FHIR\nnotes: >-\n  1up FHIR authorization uses the SMART-on-FHIR scope grammar. Access is granted per\n  context (system / user / patient) and per FHIR resource type with .read / .write / .*\n  (SMART v1) or .rs / .cruds (SMART v2) permission suffixes. Bulk Data ($export) uses the\n  documented composite scope `bulk-data|user/*.rs`. The scope surface below captures the\n  documented scope verbatim plus the SMART scope patterns the platform advertises; the\n  full effective scope set is negotiated per client at registration in the 1up Dev Portal.\nschemes:\n  - name: SMARTonFHIR\n    source: fhir/1uphealth-fhir-r4-capabilitystatement.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.1up.health/oauth2/token\n\
  \      - flow: authorizationCode\n        authorizationUrl: https://auth.1up.health/oauth2/authorize/system\n        tokenUrl: https://auth.1up.health/oauth2/token\nscopes:\n  - scope: bulk-data|user/*.rs\n    description: >-\n      Documented Bulk Data (Flat FHIR) export scope granting read/search across all\n      resource types for the authorized user context. Verbatim from the OAuth docs.\n    flows: [clientCredentials]\n    sources: [https://docs.1up.health/docs/get-started/o-auth]\nscope_patterns:\n  - pattern: system/{ResourceType}.{permission}\n    description: Backend-service access to a FHIR resource type (client_credentials).\n    example: system/Patient.read\n  - pattern: user/{ResourceType}.{permission}\n    description: User-context access to a FHIR resource type.\n    example: user/*.rs\n  - pattern: patient/{ResourceType}.{permission}\n    description: Patient-context access limited to the launch/compartment patient.\n    example: patient/Observation.read\n  - pattern:\
  \ launch / launch/patient / offline_access / openid / fhirUser\n    description: SMART launch and identity context scopes for user-facing app launch.\npermission_suffixes:\n  smart_v1: [read, write, '*']\n  smart_v2: [c, r, u, d, s, rs, cruds]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1uphealth/refs/heads/main/scopes/1uphealth-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Payer
- Claims
- Patient Access
- Health Data
token_urls:
- https://auth.1up.health/oauth2/token
---
