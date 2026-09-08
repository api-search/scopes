---
api_specs:
- filename: dips-federation-service-openapi.yml
  format: yaml
  label: DIPS Federation Service
  slug: dips-federation-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-federation-service-openapi.yml
authorization_urls: []
description: ''
docs: https://dips.developer.azure-api.net/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Dips Scopes
name_suffix: OAuth Scopes
note: 'Read live, unauthenticated, from the DIPS Federation Service OpenID Connect discovery document on 2026-09-02 (saved verbatim at well-known/dips-openid-configuration.json). Descriptions are supplied by API Evangelist only where the scope name is self-describing or is documented on the Open DIPS getting-started page; scopes DIPS does not document carry description: null rather than a guess. DIPS publishes no scopes/permissions reference page.'
overview: 'DIPS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DIPS
provider_slug: dips
schemes: []
scope_count: 0
scope_names: []
scopes: []
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
summary_line: OAuth 2.0 · no documented scopes
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
token_urls: []
---
