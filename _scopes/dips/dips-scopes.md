---
api_specs:
- filename: dips-account-api-openapi.yml
  format: yaml
  label: DIPS Account API
  slug: dips-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-account-api-openapi.yml
- filename: dips-connect-api-openapi.yml
  format: yaml
  label: DIPS Connect API
  slug: dips-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-connect-api-openapi.yml
- filename: dips-consent-api-openapi.yml
  format: yaml
  label: DIPS Consent API
  slug: dips-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-consent-api-openapi.yml
- filename: dips-default-api-openapi.yml
  format: yaml
  label: DIPS * API
  slug: dips-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-default-api-openapi.yml
- filename: dips-home-api-openapi.yml
  format: yaml
  label: DIPS Home API
  slug: dips-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-home-api-openapi.yml
- filename: dips-login-api-openapi.yml
  format: yaml
  label: DIPS Login API
  slug: dips-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-login-api-openapi.yml
- filename: dips-status-api-openapi.yml
  format: yaml
  label: DIPS Status API
  slug: dips-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-status-api-openapi.yml
- filename: dips-well-known-api-openapi.yml
  format: yaml
  label: DIPS .well Known API
  slug: dips-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-well-known-api-openapi.yml
- filename: dips-user-role-api-openapi.yml
  format: yaml
  label: DIPS User Role API
  slug: dips-user-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-user-role-api-openapi.yml
authorization_urls:
- https://api.dips.no/dips.oauth/connect/authorize
description: ''
docs: https://dips.developer.azure-api.net/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Dips Scopes
name_suffix: OAuth Scopes
note: 'Read live, unauthenticated, from the DIPS Federation Service OpenID Connect discovery document on 2026-09-02 (saved verbatim at well-known/dips-openid-configuration.json). Descriptions are supplied by API Evangelist only where the scope name is self-describing or is documented on the Open DIPS getting-started page; scopes DIPS does not document carry description: null rather than a guess. DIPS publishes no scopes/permissions reference page.'
overview: 'DIPS publishes 49 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DIPS API on a user''s behalf.


  Tokens are issued from https://api.dips.no/dips.oauth/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DIPS
provider_slug: dips
schemes: []
scope_count: 49
scope_names:
- openid
- profile
- roles
- offline
- servicebroker-wardlist-api
- dips-userroles
- dips://scopes/token-exchange/saml
- dips://scopes/token-exchange/jwt
- dips-arena
- documentmanager
- dips-sb-operationplan
- dips-iam-token-attribute-service-api
- healthrecord-document:fullreadaccess
- string
- DI_PP_machinelearningdata
- APPTYPE:public
- azure-speech
- openai-whisper
- openai-gpt4o
- dips-authorization-service.external-pip
- dips-authorization-service.query/blockedforpatient
- dips-servicebroker-referralstatus-service
- HRAL
- dips-sb-gatbookings
- idmc
- dips-anc-authorizationmanager-service/*.*
- dips-anc-notificationmanager-service/*.*
- dips-anc-notificationsender-service/*.*
- dips
- dips-iam-care-relation-service-api
- dips-sb-worklist-service-api
- surgery-webport-service-api
- DI_PP_patientdata
- pas-scheduling-gatintegration
- dips-fhirr4-service-api
- launch
- dips-mobile
- dips-authorization-service.query/externaluser
- smsservice
- dips-fhir-r4
- dips-fhir
- fhir-r4
- patient/*.read
- fhirUser
- patient
- surgery-plan-service-api
- launch/patient
- MC_Logistics_PatientData
- offline_access
scopes:
- description: OpenID Connect — request an ID token for the signed-in DIPS user.
  flows: []
  scope: openid
- description: Standard OpenID Connect profile claims (name, family_name, given_name, preferred_username, ...).
  flows: []
  scope: profile
- description: Include the role claim for the authenticated user.
  flows: []
  scope: roles
- description: Legacy DIPS alias for offline access; issues a refresh token.
  flows: []
  scope: offline
- description: ''
  flows: []
  scope: servicebroker-wardlist-api
- description: Read and select the DIPS user roles available to the signed-in user (see the /userrole operations).
  flows: []
  scope: dips-userroles
- description: Exchange a SAML 2.0 assertion for a DIPS access token.
  flows: []
  scope: dips://scopes/token-exchange/saml
- description: Exchange a JWT assertion for a DIPS access token.
  flows: []
  scope: dips://scopes/token-exchange/jwt
- description: Access the DIPS Arena EHR application surface.
  flows: []
  scope: dips-arena
- description: Access the DIPS document manager service.
  flows: []
  scope: documentmanager
- description: ''
  flows: []
  scope: dips-sb-operationplan
- description: ''
  flows: []
  scope: dips-iam-token-attribute-service-api
- description: Full read access to health-record documents.
  flows: []
  scope: healthrecord-document:fullreadaccess
- description: ''
  flows: []
  scope: string
- description: ''
  flows: []
  scope: DI_PP_machinelearningdata
- description: ''
  flows: []
  scope: APPTYPE:public
- description: ''
  flows: []
  scope: azure-speech
- description: ''
  flows: []
  scope: openai-whisper
- description: ''
  flows: []
  scope: openai-gpt4o
- description: ''
  flows: []
  scope: dips-authorization-service.external-pip
- description: ''
  flows: []
  scope: dips-authorization-service.query/blockedforpatient
- description: ''
  flows: []
  scope: dips-servicebroker-referralstatus-service
- description: ''
  flows: []
  scope: HRAL
- description: ''
  flows: []
  scope: dips-sb-gatbookings
- description: Access the IDMC service.
  flows: []
  scope: idmc
- description: ''
  flows: []
  scope: dips-anc-authorizationmanager-service/*.*
- description: ''
  flows: []
  scope: dips-anc-notificationmanager-service/*.*
- description: ''
  flows: []
  scope: dips-anc-notificationsender-service/*.*
- description: ''
  flows: []
  scope: dips
- description: ''
  flows: []
  scope: dips-iam-care-relation-service-api
- description: ''
  flows: []
  scope: dips-sb-worklist-service-api
- description: ''
  flows: []
  scope: surgery-webport-service-api
- description: ''
  flows: []
  scope: DI_PP_patientdata
- description: ''
  flows: []
  scope: pas-scheduling-gatintegration
- description: Access the DIPS FHIR R4 service API.
  flows: []
  scope: dips-fhirr4-service-api
- description: SMART on FHIR EHR launch context.
  flows: []
  scope: launch
- description: Access reserved for DIPS mobile clients.
  flows: []
  scope: dips-mobile
- description: ''
  flows: []
  scope: dips-authorization-service.query/externaluser
- description: Access the DIPS SMS service.
  flows: []
  scope: smsservice
- description: Access the DIPS FHIR R4 API.
  flows: []
  scope: dips-fhir-r4
- description: Access the DIPS FHIR API (the scope named in the Open DIPS getting-started guide).
  flows: []
  scope: dips-fhir
- description: Access the FHIR R4 service.
  flows: []
  scope: fhir-r4
- description: SMART on FHIR read access to every resource in the patient compartment.
  flows: []
  scope: patient/*.read
- description: SMART on FHIR — identity of the user as a FHIR resource.
  flows: []
  scope: fhirUser
- description: SMART on FHIR patient compartment access.
  flows: []
  scope: patient
- description: ''
  flows: []
  scope: surgery-plan-service-api
- description: SMART on FHIR patient launch context.
  flows: []
  scope: launch/patient
- description: ''
  flows: []
  scope: MC_Logistics_PatientData
- description: Issue a refresh token so the client can renew access without re-prompting the user.
  flows: []
  scope: offline_access
slug: dips-scopes
source_filename: dips-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://api.dips.no/dips.oauth/.well-known/openid-configuration\ndocs: https://dips.developer.azure-api.net/getting-started\nnote: 'Read live, unauthenticated, from the DIPS Federation Service OpenID Connect discovery document on 2026-09-02\n  (saved verbatim at well-known/dips-openid-configuration.json). Descriptions are supplied by API Evangelist only\n  where the scope name is self-describing or is documented on the Open DIPS getting-started page; scopes DIPS does\n  not document carry description: null rather than a guess. DIPS publishes no scopes/permissions reference page.'\nissuer: https://api.dips.no/dips.oauth\nauthorization_endpoint: https://api.dips.no/dips.oauth/connect/authorize\ntoken_endpoint: https://api.dips.no/dips.oauth/connect/token\nintrospection_endpoint: https://api.dips.no/dips.oauth/connect/introspect\nrevocation_endpoint: https://api.dips.no/dips.oauth/connect/revocation\ngrant_types_supported:\n- authorization_code\n\
  - client_credentials\n- refresh_token\n- implicit\n- password\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:openid:params:grant-type:ciba\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:ietf:params:oauth:grant-type:saml2-bearer\n- http://dips.no/identity/2016/assertion/userroles\n- urn:dips:params:refreshaccesstoken:grant-type:jwt-bearer\n- urn:dips:federation:grant-type:user-role-change\ntoken_endpoint_auth_methods_supported:\n- client_secret_post\n- private_key_jwt\n- client_secret_basic\npkce_code_challenge_methods_supported:\n- plain\n- S256\nscope_count: 49\ndocumented_scope_count: 23\nsmart_on_fhir_scopes:\n- launch\n- launch/patient\n- patient\n- patient/*.read\n- fhirUser\n- offline_access\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token for the signed-in DIPS user.\n- name: profile\n  description: Standard OpenID Connect profile claims (name, family_name, given_name, preferred_username, ...).\n- name: roles\n  description: Include the\
  \ role claim for the authenticated user.\n- name: offline\n  description: Legacy DIPS alias for offline access; issues a refresh token.\n- name: servicebroker-wardlist-api\n  description: null\n- name: dips-userroles\n  description: Read and select the DIPS user roles available to the signed-in user (see the /userrole operations).\n- name: dips://scopes/token-exchange/saml\n  description: Exchange a SAML 2.0 assertion for a DIPS access token.\n- name: dips://scopes/token-exchange/jwt\n  description: Exchange a JWT assertion for a DIPS access token.\n- name: dips-arena\n  description: Access the DIPS Arena EHR application surface.\n- name: documentmanager\n  description: Access the DIPS document manager service.\n- name: dips-sb-operationplan\n  description: null\n- name: dips-iam-token-attribute-service-api\n  description: null\n- name: healthrecord-document:fullreadaccess\n  description: Full read access to health-record documents.\n- name: string\n  description: null\n- name: DI_PP_machinelearningdata\n\
  \  description: null\n- name: APPTYPE:public\n  description: null\n- name: azure-speech\n  description: null\n- name: openai-whisper\n  description: null\n- name: openai-gpt4o\n  description: null\n- name: dips-authorization-service.external-pip\n  description: null\n- name: dips-authorization-service.query/blockedforpatient\n  description: null\n- name: dips-servicebroker-referralstatus-service\n  description: null\n- name: HRAL\n  description: null\n- name: dips-sb-gatbookings\n  description: null\n- name: idmc\n  description: Access the IDMC service.\n- name: dips-anc-authorizationmanager-service/*.*\n  description: null\n- name: dips-anc-notificationmanager-service/*.*\n  description: null\n- name: dips-anc-notificationsender-service/*.*\n  description: null\n- name: dips\n  description: null\n- name: dips-iam-care-relation-service-api\n  description: null\n- name: dips-sb-worklist-service-api\n  description: null\n- name: surgery-webport-service-api\n  description: null\n- name: DI_PP_patientdata\n\
  \  description: null\n- name: pas-scheduling-gatintegration\n  description: null\n- name: dips-fhirr4-service-api\n  description: Access the DIPS FHIR R4 service API.\n- name: launch\n  description: SMART on FHIR EHR launch context.\n- name: dips-mobile\n  description: Access reserved for DIPS mobile clients.\n- name: dips-authorization-service.query/externaluser\n  description: null\n- name: smsservice\n  description: Access the DIPS SMS service.\n- name: dips-fhir-r4\n  description: Access the DIPS FHIR R4 API.\n- name: dips-fhir\n  description: Access the DIPS FHIR API (the scope named in the Open DIPS getting-started guide).\n- name: fhir-r4\n  description: Access the FHIR R4 service.\n- name: patient/*.read\n  description: SMART on FHIR read access to every resource in the patient compartment.\n- name: fhirUser\n  description: SMART on FHIR — identity of the user as a FHIR resource.\n- name: patient\n  description: SMART on FHIR patient compartment access.\n- name: surgery-plan-service-api\n\
  \  description: null\n- name: launch/patient\n  description: SMART on FHIR patient launch context.\n- name: MC_Logistics_PatientData\n  description: null\n- name: offline_access\n  description: Issue a refresh token so the client can renew access without re-prompting the user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/scopes/dips-scopes.yml
summary_line: 49 scopes
tags:
- Company
- Healthcare
- Electronic Health Records
- Health IT
- FHIR
- openEHR
- Interoperability
- Identity
- OpenID Connect
- Norway
- Hospitals
- SMART on FHIR
token_bound: false
token_urls:
- https://api.dips.no/dips.oauth/connect/token
---
