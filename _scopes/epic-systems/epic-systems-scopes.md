---
authorization_urls:
- https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize
description: ''
docs: https://fhir.epic.com/Documentation?docId=oauth2
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Epic Systems Scopes
name_suffix: OAuth Scopes
note: Epic authorizes its FHIR APIs with SMART on FHIR scopes layered on OAuth 2.0. The five scopes below are the base scopes advertised anonymously in the live R4 smart-configuration / openid-configuration (scopes_supported). Clinical resource access is granted with SMART v1/v2 scope grammar (both permission-v1 and permission-v2 advertised), negotiated per registered client and per connected health system - these are not enumerated in the discovery document, so the grammar and per-context patterns are documented below rather than as fixed strings.
overview: 'Epic Systems publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Epic Systems API on a user''s behalf.


  Tokens are issued from https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Epic Systems
provider_slug: epic-systems
schemes:
- flows:
  - authorizationUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token
  - flow: clientCredentials
    note: SMART Backend Services; private_key_jwt (asymmetric) client authentication; system-level scopes; backs Bulk Data $export.
    tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token
  name: SMART-on-FHIR-OAuth2
  source: fhir/epic-fhir-r4-smart-configuration.json
scope_count: 5
scope_names:
- openid
- profile
- fhirUser
- launch
- epic.scanning.dmsusername
scopes:
- description: OpenID Connect - request an id_token identifying the end user.
  flows: []
  scope: openid
- description: OpenID Connect profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Return the FHIR resource (Practitioner/Patient/RelatedPerson) representing the current user.
  flows: []
  scope: fhirUser
- description: SMART EHR-launch context (patient/encounter) passed from the Epic launch.
  flows: []
  scope: launch
- description: Epic-specific scope exposing the document-management scanning username (Epic extension).
  flows: []
  scope: epic.scanning.dmsusername
slug: epic-systems-scopes
source_filename: epic-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: fhir/epic-fhir-r4-smart-configuration.json, well-known/epic-systems-openid-configuration.json\ndocs: https://fhir.epic.com/Documentation?docId=oauth2\nnote: Epic authorizes its FHIR APIs with SMART on FHIR scopes layered on OAuth 2.0. The five scopes below\n  are the base scopes advertised anonymously in the live R4 smart-configuration / openid-configuration\n  (scopes_supported). Clinical resource access is granted with SMART v1/v2 scope grammar (both permission-v1\n  and permission-v2 advertised), negotiated per registered client and per connected health system - these\n  are not enumerated in the discovery document, so the grammar and per-context patterns are documented\n  below rather than as fixed strings.\nschemes:\n- name: SMART-on-FHIR-OAuth2\n  source: fhir/epic-fhir-r4-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/authorize\n\
  \    tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token\n    note: SMART Backend Services; private_key_jwt (asymmetric) client authentication; system-level scopes;\n      backs Bulk Data $export.\nadvertised_scopes: &id001\n- scope: openid\n  description: OpenID Connect - request an id_token identifying the end user.\n- scope: profile\n  description: OpenID Connect profile claims for the authenticated user.\n- scope: fhirUser\n  description: Return the FHIR resource (Practitioner/Patient/RelatedPerson) representing the current\n    user.\n- scope: launch\n  description: SMART EHR-launch context (patient/encounter) passed from the Epic launch.\n- scope: epic.scanning.dmsusername\n  description: Epic-specific scope exposing the document-management scanning username (Epic extension).\nscope_grammar:\n  detail: Clinical access uses SMART scopes of the form\
  \ <context>/<Resource>.<access>. Context prefixes\n    - patient/ (single in-context patient), user/ (everything the authenticated user may see), system/\n    (backend, no user, for client_credentials). Access - SMART v1 uses .read / .write / .* ; SMART v2\n    uses granular .c (create) .r (read) .u (update) .d (delete) .s (search), e.g. patient/Observation.rs.\n  examples:\n  - patient/Patient.read\n  - patient/Observation.read\n  - patient/MedicationRequest.read\n  - user/Encounter.read\n  - system/Patient.read\n  - system/Group.read\n  additional:\n  - offline_access\n  resources_scopable: 59 R4 resource types (see data-model/epic-systems-data-model.yml); STU3 (35) and\n    DSTU2 (17) expose narrower sets.\nscopes: *id001\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-systems/refs/heads/main/scopes/epic-systems-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- United States
- Electronic Health Records
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- US Core
- Clinical Data
token_bound: false
token_urls:
- https://fhir.epic.com/interconnect-fhir-oauth/oauth2/token
---
