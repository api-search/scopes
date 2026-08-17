---
api_specs:
- filename: health-gorilla-binary-api-openapi.yml
  format: yaml
  label: Health Gorilla Binary API
  slug: health-gorilla-binary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-binary-api-openapi.yml
- filename: health-gorilla-capabilitystatement-api-openapi.yml
  format: yaml
  label: Health Gorilla CapabilityStatement API
  slug: health-gorilla-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-capabilitystatement-api-openapi.yml
- filename: health-gorilla-coverage-api-openapi.yml
  format: yaml
  label: Health Gorilla Coverage API
  slug: health-gorilla-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-coverage-api-openapi.yml
- filename: health-gorilla-diagnosticreport-api-openapi.yml
  format: yaml
  label: Health Gorilla DiagnosticReport API
  slug: health-gorilla-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-diagnosticreport-api-openapi.yml
- filename: health-gorilla-documentreference-api-openapi.yml
  format: yaml
  label: Health Gorilla DocumentReference API
  slug: health-gorilla-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-documentreference-api-openapi.yml
- filename: health-gorilla-observation-api-openapi.yml
  format: yaml
  label: Health Gorilla Observation API
  slug: health-gorilla-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-observation-api-openapi.yml
- filename: health-gorilla-patient-api-openapi.yml
  format: yaml
  label: Health Gorilla Patient API
  slug: health-gorilla-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-patient-api-openapi.yml
- filename: health-gorilla-practitioner-api-openapi.yml
  format: yaml
  label: Health Gorilla Practitioner API
  slug: health-gorilla-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-practitioner-api-openapi.yml
- filename: health-gorilla-requestgroup-api-openapi.yml
  format: yaml
  label: Health Gorilla RequestGroup API
  slug: health-gorilla-requestgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-requestgroup-api-openapi.yml
- filename: health-gorilla-servicerequest-api-openapi.yml
  format: yaml
  label: Health Gorilla ServiceRequest API
  slug: health-gorilla-servicerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-servicerequest-api-openapi.yml
authorization_urls:
- https://www.healthgorilla.com/oauth/authorize
description: 'Health Gorilla''s OAuth scope surface is published in two places: the SMART App Launch configuration served anonymously from the API host, which enumerates the scopes the authorization server supports, and the Scopes & Access Control guide, which describes how scopes are assigned and enforced. Scopes are fixed at client registration — a client may request only scopes assigned during onboarding, cannot self-assign, cannot expand scope during token exchange, and cannot expand scope on refresh. The OpenAPI in openapi/ declares only a bearer http scheme with no oauth2 flows, so none of this is derivable from the spec; every scope below comes from the provider''s own discovery document or docs.'
docs: https://developer.healthgorilla.com/docs/scopes-access-control
flows:
- authorizationCode
- implicit
- clientCredentials
- jwtBearer
kind: oauth-scopes
layout: scope
method: searched
name: Health Gorilla Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Health Gorilla publishes 11 OAuth 2.0 scopes via the authorizationCode, implicit, clientCredentials, and jwtBearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Health Gorilla API on a user''s behalf.


  Tokens are issued from https://www.healthgorilla.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Health Gorilla
provider_slug: health-gorilla
schemes:
- flows:
  - authorizationUrl: https://www.healthgorilla.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.healthgorilla.com/oauth/token
  - authorizationUrl: https://www.healthgorilla.com/oauth/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://www.healthgorilla.com/oauth/token
  - flow: jwtBearer
    tokenUrl: https://www.healthgorilla.com/oauth/token
  name: SMARTonFHIR
  source: well-known/health-gorilla-smart-configuration.json
  type: oauth2
scope_count: 11
scope_names:
- user/*.*
- system/*.*
- offline_access
- openid
- profile
- fhirUser
- patient360
- rls
- nlp
- create_users
- place_orders
scopes:
- description: SMART user-level access. Grants the app the intersection of the client's registered scopes and the authenticated user's permissions within the tenant.
  flows:
  - authorizationCode
  - implicit
  scope: user/*.*
- description: SMART backend-services (system) access for server-to-server integrations with no interactive user.
  flows:
  - clientCredentials
  - jwtBearer
  scope: system/*.*
- description: Requests a refresh token so the client can renew access without re-authorizing.
  flows:
  - authorizationCode
  scope: offline_access
- description: Enables OpenID Connect single sign-on and issuance of an id_token.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Releases the user profile claims (name, given_name, family_name, birthdate, gender).
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Releases the fhirUser claim identifying the FHIR resource for the authenticated user.
  flows:
  - authorizationCode
  - implicit
  scope: fhirUser
- description: Health Gorilla proprietary scope gating the Patient360 record-retrieval product ($p360-retrieve / $p360-search on DocumentReference and Patient).
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient360
- description: Health Gorilla proprietary scope for the Record Locator Service, which locates where a patient's records exist across the network before retrieval.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rls
- description: Health Gorilla proprietary scope for natural-language / OCR processing of retrieved clinical documents (see the DocumentReference $ocr operation).
  flows:
  - authorizationCode
  - clientCredentials
  scope: nlp
- description: Permits provisioning of Health Gorilla users. Named in the Scopes & Access Control guide as an example of a per-integration scope assigned at registration; it is not advertised in the SMART configuration.
  flows:
  - authorizationCode
  - clientCredentials
  scope: create_users
- description: Permits submission of diagnostic (lab / radiology) orders. Appears as the granted scope in the token response example in the OAuth 2.0 Authentication reference; it is not advertised in the SMART configuration.
  flows:
  - authorizationCode
  - clientCredentials
  scope: place_orders
slug: health-gorilla-scopes
source_filename: health-gorilla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://api.healthgorilla.com/.well-known/smart-configuration\ndocs: https://developer.healthgorilla.com/docs/scopes-access-control\ndescription: >-\n  Health Gorilla's OAuth scope surface is published in two places: the SMART App\n  Launch configuration served anonymously from the API host, which enumerates\n  the scopes the authorization server supports, and the Scopes & Access Control\n  guide, which describes how scopes are assigned and enforced. Scopes are fixed\n  at client registration — a client may request only scopes assigned during\n  onboarding, cannot self-assign, cannot expand scope during token exchange, and\n  cannot expand scope on refresh. The OpenAPI in openapi/ declares only a bearer\n  http scheme with no oauth2 flows, so none of this is derivable from the spec;\n  every scope below comes from the provider's own discovery document or docs.\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  source: well-known/health-gorilla-smart-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.healthgorilla.com/oauth/authorize\n    tokenUrl: https://www.healthgorilla.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://www.healthgorilla.com/oauth/authorize\n  - flow: clientCredentials\n    tokenUrl: https://www.healthgorilla.com/oauth/token\n  - flow: jwtBearer\n    tokenUrl: https://www.healthgorilla.com/oauth/token\nscopes:\n- scope: user/*.*\n  family: smart\n  description: >-\n    SMART user-level access. Grants the app the intersection of the client's\n    registered scopes and the authenticated user's permissions within the tenant.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n- scope: system/*.*\n  family: smart\n  description: >-\n    SMART backend-services (system) access for server-to-server integrations\n    with no interactive user.\n  flows: [clientCredentials, jwtBearer]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n\
  - scope: offline_access\n  family: smart\n  description: Requests a refresh token so the client can renew access without re-authorizing.\n  flows: [authorizationCode]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n- scope: openid\n  family: oidc\n  description: Enables OpenID Connect single sign-on and issuance of an id_token.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/health-gorilla-smart-configuration.json, well-known/health-gorilla-openid-configuration.json]\n- scope: profile\n  family: oidc\n  description: Releases the user profile claims (name, given_name, family_name, birthdate, gender).\n  flows: [authorizationCode, implicit]\n  sources: [well-known/health-gorilla-smart-configuration.json, well-known/health-gorilla-openid-configuration.json]\n- scope: fhirUser\n  family: oidc\n  description: Releases the fhirUser claim identifying the FHIR resource for the authenticated user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/health-gorilla-smart-configuration.json,\
  \ well-known/health-gorilla-openid-configuration.json]\n- scope: patient360\n  family: health-gorilla\n  description: >-\n    Health Gorilla proprietary scope gating the Patient360 record-retrieval\n    product ($p360-retrieve / $p360-search on DocumentReference and Patient).\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n- scope: rls\n  family: health-gorilla\n  description: >-\n    Health Gorilla proprietary scope for the Record Locator Service, which\n    locates where a patient's records exist across the network before retrieval.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n- scope: nlp\n  family: health-gorilla\n  description: >-\n    Health Gorilla proprietary scope for natural-language / OCR processing of\n    retrieved clinical documents (see the DocumentReference $ocr operation).\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/health-gorilla-smart-configuration.json]\n\
  - scope: create_users\n  family: health-gorilla\n  description: >-\n    Permits provisioning of Health Gorilla users. Named in the Scopes & Access\n    Control guide as an example of a per-integration scope assigned at\n    registration; it is not advertised in the SMART configuration.\n  flows: [authorizationCode, clientCredentials]\n  sources: ['https://developer.healthgorilla.com/docs/scopes-access-control']\n- scope: place_orders\n  family: health-gorilla\n  description: >-\n    Permits submission of diagnostic (lab / radiology) orders. Appears as the\n    granted scope in the token response example in the OAuth 2.0 Authentication\n    reference; it is not advertised in the SMART configuration.\n  flows: [authorizationCode, clientCredentials]\n  sources: ['https://developer.healthgorilla.com/reference/oauth-20-authentication']\nenforcement:\n  assignment: >-\n    Scopes are configured at registration and bound to a specific client_id.\n    Additional API access requires a scope change\
  \ requested through Health Gorilla.\n  request_format: space-delimited list on the scope parameter\n  default_behavior: >-\n    If scope is omitted from the authorization request, the client's registered\n    default scopes are applied.\n  downscoping: The authorization server may issue a token with a subset of the requested scopes.\n  expansion: >-\n    Scope cannot be expanded during token exchange or refresh. For the\n    authorization code grant, the granted scope cannot exceed the scope requested\n    in the original authorization request.\n  two_layer_model: >-\n    OAuth scopes govern which APIs the client may call; user-level permissions\n    govern what data and operations are permitted inside the tenant. Both must be\n    satisfied. Scopes never grant access outside the token's tenant context.\n  failures: [insufficient_scope, invalid_client, invalid_grant]\ncompleteness:\n  note: >-\n    Health Gorilla does not publish an exhaustive scope reference. The SMART\n    configuration\
  \ lists nine supported scopes and the docs name two further\n    per-integration scopes by example, stating explicitly that \"the exact scopes\n    available to a client are defined at registration time and vary by\n    integration.\" No additional scopes were invented to fill the gap.\n  advertised_in_discovery: 9\n  named_in_docs_only: 2\nx-evidence:\n- {url: 'https://api.healthgorilla.com/.well-known/smart-configuration', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://developer.healthgorilla.com/docs/scopes-access-control.md', http_status: 200, fetched: '2026-08-14'}\n- {url: 'https://developer.healthgorilla.com/reference/oauth-20-authentication.md', http_status: 200, fetched: '2026-08-14'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/scopes/health-gorilla-scopes.yml
summary_line: 11 scopes · authorizationCode/implicit/clientCredentials/jwtBearer
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
- TEFCA
- QHIN
- Health Information Exchange
- Lab Results
- Clinical Documents
- SMART on FHIR
- Patient Records
- HL7
token_urls:
- https://www.healthgorilla.com/oauth/token
---
