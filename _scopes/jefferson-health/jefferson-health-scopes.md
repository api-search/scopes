---
api_specs:
- filename: jefferson-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Jefferson Health Allergy Intolerance API
  slug: jefferson-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-allergy-intolerance-api-openapi.yml
- filename: jefferson-health-bulk-data-api-openapi.yml
  format: yaml
  label: Jefferson Health Bulk Data API
  slug: jefferson-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-bulk-data-api-openapi.yml
- filename: jefferson-health-condition-api-openapi.yml
  format: yaml
  label: Jefferson Health Condition API
  slug: jefferson-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-condition-api-openapi.yml
- filename: jefferson-health-document-reference-api-openapi.yml
  format: yaml
  label: Jefferson Health Document Reference API
  slug: jefferson-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-document-reference-api-openapi.yml
- filename: jefferson-health-encounter-api-openapi.yml
  format: yaml
  label: Jefferson Health Encounter API
  slug: jefferson-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-encounter-api-openapi.yml
- filename: jefferson-health-endpoint-api-openapi.yml
  format: yaml
  label: Jefferson Health Endpoint API
  slug: jefferson-health-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-endpoint-api-openapi.yml
- filename: jefferson-health-healthcare-service-api-openapi.yml
  format: yaml
  label: Jefferson Health Healthcare Service API
  slug: jefferson-health-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-healthcare-service-api-openapi.yml
- filename: jefferson-health-insurance-plan-api-openapi.yml
  format: yaml
  label: Jefferson Health Insurance Plan API
  slug: jefferson-health-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-insurance-plan-api-openapi.yml
- filename: jefferson-health-location-api-openapi.yml
  format: yaml
  label: Jefferson Health Location API
  slug: jefferson-health-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-location-api-openapi.yml
- filename: jefferson-health-medication-request-api-openapi.yml
  format: yaml
  label: Jefferson Health Medication Request API
  slug: jefferson-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-medication-request-api-openapi.yml
- filename: jefferson-health-metadata-api-openapi.yml
  format: yaml
  label: Jefferson Health Metadata API
  slug: jefferson-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-metadata-api-openapi.yml
- filename: jefferson-health-observation-api-openapi.yml
  format: yaml
  label: Jefferson Health Observation API
  slug: jefferson-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-observation-api-openapi.yml
- filename: jefferson-health-organization-api-openapi.yml
  format: yaml
  label: Jefferson Health Organization API
  slug: jefferson-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-organization-api-openapi.yml
- filename: jefferson-health-patient-api-openapi.yml
  format: yaml
  label: Jefferson Health Patient API
  slug: jefferson-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-patient-api-openapi.yml
- filename: jefferson-health-practitioner-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner API
  slug: jefferson-health-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-api-openapi.yml
- filename: jefferson-health-practitioner-role-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner Role API
  slug: jefferson-health-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-role-api-openapi.yml
authorization_urls:
- https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
description: 'SMART on FHIR scope surface for the Thomas Jefferson University Hospital FHIR R4 endpoint. Note the important discrepancy recorded below: the server''s own discovery document advertises only five scopes in scopes_supported, none of them resource scopes. The patient/, user/ and system/ resource scopes are real and required, but they are granted per registered application at Epic rather than enumerated in discovery — so an agent that trusts scopes_supported alone will conclude, wrongly, that no clinical data can be requested.'
docs:
- https://fhir.epic.com/Documentation
- https://hl7.org/fhir/smart-app-launch/scopes-and-launch-context.html
- https://www.jeffersonhealthplans.com/home/about-us/interoperability/authentication-and-data-endpoints/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Jefferson Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jefferson Health publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jefferson Health API on a user''s behalf.


  Tokens are issued from https://fhir.jefferson.edu/FHIRProxy/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jefferson Health
provider_slug: jefferson-health
schemes:
- description: SMART App Launch / OAuth 2.0 with mandatory PKCE (S256) for patient-facing standalone launches and provider-facing EHR launches.
  flows:
  - authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token
  issuer: https://fhir.jefferson.edu/FHIRProxy/oauth2
  name: smartOnFhir
  scope_syntax_evidence: smart-configuration capabilities include both permission-v1 and permission-v2, so patient/Observation.read and patient/Observation.rs are both accepted.
  scope_syntax_supported:
  - v1
  - v2
  server: tjuh-fhir-r4
  source: well-known/jefferson-health-tjuh-smart-configuration.json
scope_count: 15
scope_names:
- openid
- profile
- fhirUser
- launch
- epic.scanning.dmsusername
- offline_access
- patient/Patient.read
- patient/Observation.read
- patient/Condition.read
- patient/Encounter.read
- patient/MedicationRequest.read
- patient/AllergyIntolerance.read
- patient/DocumentReference.read
- user/Patient.read
- system/Patient.read
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Identity of the user launching the app, as a FHIR resource reference.
  flows:
  - authorizationCode
  scope: fhirUser
- description: EHR launch context for provider-launched apps.
  flows:
  - authorizationCode
  scope: launch
- description: Epic-proprietary scope for document-management-system username exchange. Not part of SMART App Launch; advertised by this server.
  flows:
  - authorizationCode
  scope: epic.scanning.dmsusername
- description: Refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read the launching patient's demographics.
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: Read the launching patient's observations (labs, vitals).
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read the launching patient's conditions, problems and diagnoses.
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read the launching patient's encounters.
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read the launching patient's medication requests.
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read the launching patient's allergies and intolerances.
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: Read the launching patient's clinical documents and notes.
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: Read Patient as the launching user (provider context).
  flows:
  - authorizationCode
  scope: user/Patient.read
- description: System-level Patient read for backend services, used by the Bulk Data group export.
  flows:
  - clientCredentials
  - jwtBearer
  scope: system/Patient.read
slug: jefferson-health-scopes
source_filename: jefferson-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4/.well-known/smart-configuration\n  and .../.well-known/openid-configuration (fetched 2026-08-15, HTTP 200), merged\n  with the oauth2 scope map declared in\n  openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml. Supersedes the\n  2026-07-11 derived-only pass.\ndocs:\n  - https://fhir.epic.com/Documentation\n  - https://hl7.org/fhir/smart-app-launch/scopes-and-launch-context.html\n  - https://www.jeffersonhealthplans.com/home/about-us/interoperability/authentication-and-data-endpoints/\ndescription: >-\n  SMART on FHIR scope surface for the Thomas Jefferson University Hospital FHIR\n  R4 endpoint. Note the important discrepancy recorded below: the server's own\n  discovery document advertises only five scopes in scopes_supported, none of\n  them resource scopes. The patient/, user/ and system/ resource scopes are real\n  and required, but they are granted per registered\
  \ application at Epic rather\n  than enumerated in discovery — so an agent that trusts scopes_supported alone\n  will conclude, wrongly, that no clinical data can be requested.\n\nschemes:\n  - name: smartOnFhir\n    server: tjuh-fhir-r4\n    issuer: https://fhir.jefferson.edu/FHIRProxy/oauth2\n    source: well-known/jefferson-health-tjuh-smart-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize\n        tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token\n    description: >-\n      SMART App Launch / OAuth 2.0 with mandatory PKCE (S256) for patient-facing\n      standalone launches and provider-facing EHR launches.\n    scope_syntax_supported: [v1, v2]\n    scope_syntax_evidence: >-\n      smart-configuration capabilities include both permission-v1 and\n      permission-v2, so patient/Observation.read and patient/Observation.rs are\n      both accepted.\n\nadvertised_scopes_supported:\n\
  \  source: https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4/.well-known/smart-configuration\n  probed: '2026-08-15'\n  http_status: 200\n  scopes:\n    - epic.scanning.dmsusername\n    - fhirUser\n    - launch\n    - openid\n    - profile\n  note: >-\n    This is the complete scopes_supported array the server publishes. It contains\n    no resource scopes at all, and includes one Epic-proprietary scope\n    (epic.scanning.dmsusername) that is not part of SMART App Launch.\n\nscopes:\n  # --- identity / launch context, confirmed in the live discovery document ---\n  - scope: openid\n    description: OpenID Connect authentication.\n    kind: identity\n    flows: [authorizationCode]\n    advertised: true\n    sources:\n      - well-known/jefferson-health-tjuh-smart-configuration.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n  - scope: profile\n    description: OpenID Connect profile claims.\n    kind: identity\n    flows: [authorizationCode]\n    advertised:\
  \ true\n    sources: [well-known/jefferson-health-tjuh-smart-configuration.json]\n  - scope: fhirUser\n    description: Identity of the user launching the app, as a FHIR resource reference.\n    kind: identity\n    flows: [authorizationCode]\n    advertised: true\n    sources:\n      - well-known/jefferson-health-tjuh-smart-configuration.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n  - scope: launch\n    description: EHR launch context for provider-launched apps.\n    kind: launch-context\n    flows: [authorizationCode]\n    advertised: true\n    sources:\n      - well-known/jefferson-health-tjuh-smart-configuration.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n  - scope: epic.scanning.dmsusername\n    description: >-\n      Epic-proprietary scope for document-management-system username exchange.\n      Not part of SMART App Launch; advertised by this server.\n    kind: vendor-proprietary\n    flows: [authorizationCode]\n\
  \    advertised: true\n    sources: [well-known/jefferson-health-tjuh-smart-configuration.json]\n  - scope: offline_access\n    description: Refresh token for long-lived access.\n    kind: launch-context\n    flows: [authorizationCode]\n    advertised: false\n    advertised_note: >-\n      Not in scopes_supported, but the server declares the permission-offline\n      SMART capability and grant_types_supported includes refresh_token.\n    sources:\n      - well-known/jefferson-health-tjuh-smart-configuration.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n\n  # --- resource scopes: real, required, NOT advertised in discovery ---\n  - scope: patient/Patient.read\n    description: Read the launching patient's demographics.\n    kind: patient-resource\n    resource: Patient\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/Observation.read\n    description:\
  \ Read the launching patient's observations (labs, vitals).\n    kind: patient-resource\n    resource: Observation\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/Condition.read\n    description: Read the launching patient's conditions, problems and diagnoses.\n    kind: patient-resource\n    resource: Condition\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/Encounter.read\n    description: Read the launching patient's encounters.\n    kind: patient-resource\n    resource: Encounter\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/MedicationRequest.read\n    description: Read the launching patient's medication requests.\n    kind: patient-resource\n    resource: MedicationRequest\n\
  \    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/AllergyIntolerance.read\n    description: Read the launching patient's allergies and intolerances.\n    kind: patient-resource\n    resource: AllergyIntolerance\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: patient/DocumentReference.read\n    description: Read the launching patient's clinical documents and notes.\n    kind: patient-resource\n    resource: DocumentReference\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n  - scope: user/Patient.read\n    description: Read Patient as the launching user (provider context).\n    kind: user-resource\n    resource: Patient\n    flows: [authorizationCode]\n    advertised: false\n    sources: [openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml]\n\
  \  - scope: system/Patient.read\n    description: >-\n      System-level Patient read for backend services, used by the Bulk Data\n      group export.\n    kind: system-resource\n    resource: Patient\n    flows: [clientCredentials, jwtBearer]\n    advertised: false\n    advertised_note: >-\n      Backed by grant_types_supported client_credentials +\n      urn:ietf:params:oauth:grant-type:jwt-bearer and private_key_jwt client\n      authentication in the live discovery document.\n    sources:\n      - well-known/jefferson-health-tjuh-openid-configuration.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n\nscope_count: 15\nadvertised_scope_count: 5\n\njhp_provider_directory:\n  server: https://providerfhirapi.healthpartnersplans.com\n  scopes: []\n  note: >-\n    No scopes. The Da Vinci Plan-Net directory is anonymous — verified with an\n    unauthenticated HTTP 200 on GET /Practitioner?_count=2. Its\n    CapabilityStatement advertises SMART oauth-uris pointing\
  \ at\n    appgallery.healthpartnersplans.com, but those belong to the separate\n    Jefferson Health Plans Patient Access API.\n\ngaps:\n  - >-\n    Neither Jefferson Health nor Jefferson Health Plans publishes a scopes or\n    permissions reference page of its own. Integrators are pointed at Epic's\n    generic documentation and at the per-app scope selection in the Epic on FHIR\n    app registration form, so the authoritative scope list for any given\n    application is visible only inside that application's own registration.\n  - >-\n    The Jefferson Health Plans Patient Access API scope set could not be probed:\n    its SMART configuration endpoint returns an HTML portal shell rather than a\n    discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/scopes/jefferson-health-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
token_urls:
- https://fhir.jefferson.edu/FHIRProxy/oauth2/token
---
