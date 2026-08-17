---
api_specs:
- filename: temple-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Temple Health Allergy Intolerance API
  slug: temple-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-allergy-intolerance-api-openapi.yml
- filename: temple-health-bulk-data-api-openapi.yml
  format: yaml
  label: Temple Health Bulk Data API
  slug: temple-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-bulk-data-api-openapi.yml
- filename: temple-health-condition-api-openapi.yml
  format: yaml
  label: Temple Health Condition API
  slug: temple-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-condition-api-openapi.yml
- filename: temple-health-document-reference-api-openapi.yml
  format: yaml
  label: Temple Health Document Reference API
  slug: temple-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-document-reference-api-openapi.yml
- filename: temple-health-encounter-api-openapi.yml
  format: yaml
  label: Temple Health Encounter API
  slug: temple-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-encounter-api-openapi.yml
- filename: temple-health-medication-request-api-openapi.yml
  format: yaml
  label: Temple Health Medication Request API
  slug: temple-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-medication-request-api-openapi.yml
- filename: temple-health-metadata-api-openapi.yml
  format: yaml
  label: Temple Health Metadata API
  slug: temple-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-metadata-api-openapi.yml
- filename: temple-health-observation-api-openapi.yml
  format: yaml
  label: Temple Health Observation API
  slug: temple-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-observation-api-openapi.yml
- filename: temple-health-patient-api-openapi.yml
  format: yaml
  label: Temple Health Patient API
  slug: temple-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-patient-api-openapi.yml
authorization_urls:
- https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Temple Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Temple Health publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Temple Health API on a user''s behalf.


  Tokens are issued from https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Temple Health
provider_slug: temple-health
schemes:
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-allergy-intolerance-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-bulk-data-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-condition-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-document-reference-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-encounter-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-medication-request-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-metadata-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-observation-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  source: openapi/temple-health-patient-api-openapi.yml
scope_count: 15
scope_names:
- epic.scanning.dmsusername
- fhirUser
- launch
- offline_access
- openid
- patient/AllergyIntolerance.read
- patient/Condition.read
- patient/DocumentReference.read
- patient/Encounter.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
- profile
- system/Patient.read
- user/Patient.read
scopes:
- description: Epic vendor-specific scope for document-management scanning user context. Epic-proprietary, not part of SMART App Launch.
  flows:
  - authorizationCode
  scope: epic.scanning.dmsusername
- description: Identity of the user launching the app
  flows:
  - authorizationCode
  scope: fhirUser
- description: EHR launch context for provider-launched apps
  flows:
  - authorizationCode
  scope: launch
- description: Refresh token for long-lived access
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Read the launching patient's allergies
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: Read the launching patient's conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read the launching patient's documents
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: Read the launching patient's encounters
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read the launching patient's medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read the launching patient's observations
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read the launching patient's demographics
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: OpenID Connect profile claim for the launching user
  flows:
  - authorizationCode
  scope: profile
- description: System-level Patient read (Bulk Data)
  flows:
  - authorizationCode
  scope: system/Patient.read
- description: Read Patient as the launching user
  flows:
  - authorizationCode
  scope: user/Patient.read
slug: temple-health-scopes
source_filename: temple-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: Live GET https://epicaccess.templehealth.org/FhirProxyPrd/api/FHIR/R4/.well-known/smart-configuration\n  and .../FhirProxyPrd/oauth2/.well-known/openid-configuration (both HTTP 200, 2026-08-15), reconciled\n  against the oauth2 securitySchemes in openapi/*.yml.\ndocs: null\ndiscovery:\n  smart_configuration: https://epicaccess.templehealth.org/FhirProxyPrd/api/FHIR/R4/.well-known/smart-configuration\n  openid_configuration: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/.well-known/openid-configuration\n  issuer: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2\n  authorization_endpoint: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n  token_endpoint: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  code_challenge_methods_supported:\n  - S256\n  smart_capabilities:\n  - launch-ehr\n  - launch-standalone\n  - client-public\n  - client-confidential-symmetric\n  - client-confidential-asymmetric\n  - context-banner\n  - context-style\n  - context-ehr-patient\n  - context-ehr-encounter\n  - context-standalone-patient\n  - permission-offline\n  - permission-patient\n  - permission-user\n  - permission-v1\n  - permission-v2\n  - sso-openid-connect\n  - authorize-post\nserver_declared_scopes_supported:\n- epic.scanning.dmsusername\n- fhirUser\n- launch\n- openid\n- profile\ndiscrepancy: 'IMPORTANT: the server''s own scopes_supported list contains only five values and does NOT\n  enumerate any patient/*, user/* or system/* clinical scope — even though it declares the permission-patient,\n  permission-user, permission-offline, permission-v1 and permission-v2 SMART capabilities,\
  \ which mean\n  those scope families ARE grantable. scopes_supported on this endpoint is therefore incomplete as a machine-readable\n  grant list: a client that trusted it would conclude no clinical data is reachable. The clinical scopes\n  below come from the OpenAPI security requirements and the SMART App Launch scope syntax the declared\n  capabilities commit to.'\nschemes:\n- name: smartOnFhir\n  source: openapi/temple-health-allergy-intolerance-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-bulk-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl:\
  \ https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-condition-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-document-reference-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-encounter-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-medication-request-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-metadata-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description:\
  \ SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-observation-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n- name: smartOnFhir\n  source: openapi/temple-health-patient-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\nscope_count: 15\nscopes:\n- scope: epic.scanning.dmsusername\n  description: Epic vendor-specific scope for document-management\
  \ scanning user context. Epic-proprietary,\n    not part of SMART App Launch.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/temple-health-smart-configuration.json\n  method: probed\n  vendor_specific: true\n- scope: fhirUser\n  description: Identity of the user launching the app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: launch\n  description: EHR launch context for provider-launched apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n\
  \  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: offline_access\n  description: Refresh token for long-lived access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n\
  \  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: openid\n  description: OpenID Connect authentication\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/AllergyIntolerance.read\n  description: Read the launching patient's allergies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n\
  \  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/Condition.read\n  description: Read the launching patient's conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method:\
  \ derived\n- scope: patient/DocumentReference.read\n  description: Read the launching patient's documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/Encounter.read\n  description: Read the launching patient's encounters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n\
  \  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/MedicationRequest.read\n  description: Read the launching patient's medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/Observation.read\n\
  \  description: Read the launching patient's observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: patient/Patient.read\n  description: Read the launching patient's demographics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n\
  \  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: profile\n  description: OpenID Connect profile claim for the launching user\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/temple-health-smart-configuration.json\n  method: probed\n- scope: system/Patient.read\n  description: System-level Patient read (Bulk Data)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n\
  \  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\n- scope: user/Patient.read\n  description: Read Patient as the launching user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\n  method: derived\nnotes:\n- 'Scope syntax is SMART App Launch: <context>/<Resource>.<permission>. permission-v1 (.read/.write) and\n  permission-v2 (.rs/.cruds) are BOTH declared, so either syntax is accepted.'\n- offline_access is declared via the permission-offline capability and is required for refresh\
  \ tokens.\n- system/* scopes apply only to the SMART Backend Services path (client_credentials + private_key_jwt)\n  used for Bulk Data, not to patient-facing apps.\n- No published scope reference page exists. Temple Health documents no scopes; Epic documents the scope\n  model generally at https://fhir.epic.com/Documentation. The endpoint itself is the only Temple-specific\n  source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/scopes/temple-health-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- Academic Medical Center
- CMS Interoperability
- Cures Act
- DSTU2
- Epic
- FHIR
- Fox Chase Cancer Center
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
token_urls:
- https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
---
