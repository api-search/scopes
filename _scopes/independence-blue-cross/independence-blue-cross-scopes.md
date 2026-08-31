---
api_specs:
- filename: independence-blue-cross-formulary-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Formulary API
  slug: independence-blue-cross-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-formulary-api-openapi.yml
- filename: independence-blue-cross-patient-access-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Patient Access API
  slug: independence-blue-cross-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-patient-access-api-openapi.yml
- filename: independence-blue-cross-provider-directory-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Provider Directory API
  slug: independence-blue-cross-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-provider-directory-api-openapi.yml
authorization_urls:
- https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Independence Blue Cross Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Independence Blue Cross publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Independence Blue Cross API on a user''s behalf.


  Tokens are issued from https://eapics.ibx.com/oauth2/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Independence Blue Cross
provider_slug: independence-blue-cross
schemes:
- flows:
  - authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://eapics.ibx.com/oauth2/v2/token
  name: smart_on_fhir
  source: openapi/_original/independence-blue-cross-patient-openapi.yml
scope_count: 4
scope_names:
- launch/patient
- patient/*.read
- openid
- offline_access
scopes:
- description: SMART standalone launch with a single patient context. The issued token is bound to exactly one member, so type-level searches return only that member's resources.
  flows:
  - authorizationCode
  scope: launch/patient
- description: Read every patient-scoped FHIR R4 resource the Patient Access API exposes — Patient, Coverage, ExplanationOfBenefit, AllergyIntolerance, CarePlan, Condition, DiagnosticReport, Encounter, Goal, Immunization, Medication, MedicationDispense, MedicationRequest, Observation and Procedure. This is a wildcard read scope; there is no published narrower per-resource alternative.
  flows:
  - authorizationCode
  scope: patient/*.read
- description: OpenID Connect identity for the authenticating member.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the application can continue reading after the access token expires without re-prompting the member. Token lifetimes are not published, so this is effectively required for any non-interactive refresh.
  flows:
  - authorizationCode
  scope: offline_access
slug: independence-blue-cross-scopes
source_filename: independence-blue-cross-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  openapi/_original/independence-blue-cross-patient-openapi.yml,\n  https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration (HTTP 200, live probe 2026-08-15)\ndocs: null\ndocs_note: >-\n  Independence Blue Cross publishes NO scopes or permissions reference page. devportal.ibx.com is a\n  JavaScript-rendered single-page application serving no content to a non-executing client, and the\n  public developer-resources page names only \"OAuth 2.0/Open ID Connect\" without enumerating scopes.\n  The scope list below is therefore the union of the OpenAPI securityScheme and the capability flags in\n  the live SMART configuration — not a provider-published reference.\nprevious_method: derived\nupgrade_note: >-\n  Upgraded from derived to probed by fetching the live SMART configuration and reconciling its\n  capability flags against the four scopes declared in the spec. No scope was added that is not\n  corroborated by\
  \ one of those two sources.\nprofile: SMART App Launch 1.0.0\napplies_to: Independence Blue Cross Patient Access API only\napplies_to_note: >-\n  The Provider Directory and Drug Formulary APIs are public and unauthenticated; they have no scope\n  surface at all. See authentication/independence-blue-cross-authentication.yml.\nschemes:\n  - name: smart_on_fhir\n    source: openapi/_original/independence-blue-cross-patient-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n        tokenUrl: https://eapics.ibx.com/oauth2/v2/token\nscopes:\n  - scope: launch/patient\n    description: >-\n      SMART standalone launch with a single patient context. The issued token is bound to exactly one\n      member, so type-level searches return only that member's resources.\n    category: launch-context\n    flows:\n      - authorizationCode\n    corroborated_by: 'smart-configuration capability: context-standalone-patient,\
  \ launch-standalone'\n    sources:\n      - openapi/_original/independence-blue-cross-patient-openapi.yml\n      - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration\n  - scope: patient/*.read\n    description: >-\n      Read every patient-scoped FHIR R4 resource the Patient Access API exposes — Patient, Coverage,\n      ExplanationOfBenefit, AllergyIntolerance, CarePlan, Condition, DiagnosticReport, Encounter, Goal,\n      Immunization, Medication, MedicationDispense, MedicationRequest, Observation and Procedure. This\n      is a wildcard read scope; there is no published narrower per-resource alternative.\n    category: data-read\n    grants: protected health information\n    flows:\n      - authorizationCode\n    corroborated_by: 'smart-configuration capability: permission-patient'\n    sources:\n      - openapi/_original/independence-blue-cross-patient-openapi.yml\n      - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration\n  - scope: openid\n\
  \    description: OpenID Connect identity for the authenticating member.\n    category: identity\n    flows:\n      - authorizationCode\n    corroborated_by: 'smart-configuration capability: sso-openid-connect'\n    sources:\n      - openapi/_original/independence-blue-cross-patient-openapi.yml\n      - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration\n  - scope: offline_access\n    description: >-\n      Issue a refresh token so the application can continue reading after the access token expires\n      without re-prompting the member. Token lifetimes are not published, so this is effectively\n      required for any non-interactive refresh.\n    category: session\n    flows:\n      - authorizationCode\n    corroborated_by: 'smart-configuration capability: permission-offline'\n    sources:\n      - openapi/_original/independence-blue-cross-patient-openapi.yml\n      - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration\nscope_count: 4\nwrite_scopes:\
  \ 0\nwrite_scopes_note: >-\n  There are none. All 60 published operations are GET, so no patient/*.write, user/*.* or system/*.*\n  scope exists on this surface.\nabsent_capabilities:\n  - capability: permission-user\n    implication: No user-level (provider-facing) scopes — this API is member-facing only.\n  - capability: permission-v2\n    implication: >-\n      SMART v2 granular scopes (patient/Observation.rs and friends) are not advertised. Only the v1\n      wildcard read scope is available, so an application cannot request least-privilege access to a\n      single resource type.\n  - capability: permission-offline-refresh / client-credentials\n    implication: >-\n      No SMART Backend Services / client_credentials flow. There is no bulk or system-level export\n      surface; every read is bound to one consenting member.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/scopes/independence-blue-cross-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Healthcare
- Health Insurance
- Blue Cross Blue Shield
- Managed Care
- Medicare
- Medicare Advantage
- Medicaid
- CHIP
- Commercial
- Dental
- Vision
- Behavioral Health
- Pharmacy Benefits
- Interoperability
- FHIR
- SMART On FHIR
- CMS
- Patient Access
- Provider Directory
- Drug Formulary
- Transparency In Coverage
token_urls:
- https://eapics.ibx.com/oauth2/v2/token
---
