---
api_specs:
- filename: lifen-fhir-api-openapi.json
  format: json
  label: Lifen FHIR API
  slug: lifen-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-fhir-api-openapi.json
- filename: lifen-authentication-api-openapi.json
  format: json
  label: Lifen Authentication API
  slug: lifen-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-authentication-api-openapi.json
authorization_urls: []
description: ''
docs: https://developer.lifen.fr/docs/platform-services-documentation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lifen Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lifen uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lifen
provider_slug: lifen
schemes:
- audience_production: https://production.platform-apis/
  audience_test: https://post-prod.platform-apis/
  extra_parameters:
  - description: Identifier connecting the application with a healthcare organization; obtained from the Lifen account manager.
    name: database_reference
  flow: clientCredentials
  name: client_credentials
  source: https://developer.lifen.fr/docs/machine-to-machine-communications
  token_endpoint: https://authentication.lifen.fr/v1/token
  token_endpoint_test: https://authentication.post-prod.lifen.fr/v1/token
  type: oauth2
- authorization_endpoint: https://authentication.lifen.fr/authorize
  flow: authorizationCode
  issuer: https://login.lifen.fr/
  name: sso_oidc
  source: https://authentication.lifen.fr/.well-known/oauth-authorization-server
  token_endpoint: https://authentication.lifen.fr/v1/authorization_code/token
  type: openIdConnect
scope_count: 0
scope_names: []
scopes: []
slug: lifen-scopes
source_filename: lifen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.lifen.fr/docs/machine-to-machine-communications\ndocs: https://developer.lifen.fr/docs/platform-services-documentation\nnotes: >-\n  The Lifen Platform issues OAuth 2.0 client-credentials access tokens whose `scope` claim carries a\n  space-delimited list of technical scopes. Lifen groups these behind FUNCTIONAL scopes granted per\n  application by the account manager; each functional scope expands to the technical scopes listed\n  below. The published OpenAPI does not declare an oauth2 securityScheme (it models the bearer token\n  as an apiKey header), so the scope inventory here is harvested from the per-service documentation\n  pages rather than derived from the spec.\nschemes:\n- name: client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://authentication.lifen.fr/v1/token\n  token_endpoint_test: https://authentication.post-prod.lifen.fr/v1/token\n  audience_production:\
  \ https://production.platform-apis/\n  audience_test: https://post-prod.platform-apis/\n  extra_parameters:\n  - name: database_reference\n    description: Identifier connecting the application with a healthcare organization; obtained from\n      the Lifen account manager.\n  source: https://developer.lifen.fr/docs/machine-to-machine-communications\n- name: sso_oidc\n  type: openIdConnect\n  flow: authorizationCode\n  authorization_endpoint: https://authentication.lifen.fr/authorize\n  token_endpoint: https://authentication.lifen.fr/v1/authorization_code/token\n  issuer: https://login.lifen.fr/\n  source: https://authentication.lifen.fr/.well-known/oauth-authorization-server\nfunctional_scopes:\n- scope: PATIENT_GAM_SEARCH\n  description: Access to the Patient / Encounter API Service — patient identity, coverage and\n    encounter (sejour) data within a given hospital.\n  grants:\n  - ORGANIZATION_READ\n  - PATIENT_READ\n  - PATIENT_SEARCH\n  - ENCOUNTER_READ\n  - ENCOUNTER_SEARCH\n  docs:\
  \ https://developer.lifen.fr/docs/access-patient-information\n- scope: APPOINTMENT_GAM_SEARCH\n  description: Access to the Appointment API Service — scheduled appointment data within a given\n    hospital.\n  grants:\n  - APPOINTMENT_READ\n  - APPOINTMENT_SEARCH\n  docs: https://developer.lifen.fr/docs/access-appointment-information\n- scope: SEND_TO_EHR\n  description: Access to the Send-documents-to-EHR API Service — push a medical document into a\n    hospital Electronic Health Record.\n  grants:\n  - ORGANIZATION_READ\n  - BINARY_CREATE\n  - COMMUNICATIONREQUEST_CREATE\n  - DOCUMENTREFERENCE_CREATE\n  docs: https://developer.lifen.fr/docs/send-a-document-to-the-ehr\n- scope: SEND_TO_MSS\n  description: Access to the MSS API Service — send a medical document to healthcare professionals\n    over the French MSSante secure-messaging network.\n  docs: https://developer.lifen.fr/docs/send-a-document-to-healthcare-professional\ntechnical_scopes:\n- scope: ORGANIZATION_READ\n  description:\
  \ Read an Organization (healthcare structure) resource.\n- scope: PATIENT_READ\n  description: Read a Patient resource by id.\n- scope: PATIENT_SEARCH\n  description: Search Patient resources.\n- scope: ENCOUNTER_READ\n  description: Read an Encounter (sejour) resource by id.\n- scope: ENCOUNTER_SEARCH\n  description: Search Encounter resources.\n- scope: APPOINTMENT_READ\n  description: Read an Appointment resource by id.\n- scope: APPOINTMENT_SEARCH\n  description: Search Appointment resources.\n- scope: BINARY_CREATE\n  description: Create a Binary resource (the document payload being sent).\n- scope: BINARY_READ\n  description: Read a Binary resource.\n  source: token response example, https://developer.lifen.fr/reference/authenticate-application\n- scope: BINARY_SEARCH\n  description: Search Binary resources.\n  source: token response example, https://developer.lifen.fr/reference/authenticate-application\n- scope: COMMUNICATIONREQUEST_CREATE\n  description: Create a CommunicationRequest\
  \ — the send operation for a document.\n- scope: DOCUMENTREFERENCE_CREATE\n  description: Create a DocumentReference describing the document being sent.\nsso_scopes:\n- scope: openid\n  description: OIDC base scope.\n- scope: profile\n  description: Profile claims.\n- scope: email\n  description: Email claim.\n- scope: address\n  description: Address claim.\n- scope: phone\n  description: Phone claim.\n- scope: offline_access\n  description: Refresh-token issuance.\nsso_scopes_source: https://authentication.lifen.fr/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/scopes/lifen-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- FHIR
- Interoperability
- Health Data
- Electronic Health Records
- Medical Documents
- Secure Messaging
- France
- HL7
token_urls: []
---
