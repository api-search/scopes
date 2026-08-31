---
api_specs:
- filename: sun-life-authorize-api-openapi.yml
  format: yaml
  label: Sun Life Authorize API
  slug: sun-life-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-authorize-api-openapi.yml
- filename: sun-life-callback-api-openapi.yml
  format: yaml
  label: Sun Life Callback API
  slug: sun-life-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-callback-api-openapi.yml
- filename: sun-life-coverage-api-openapi.yml
  format: yaml
  label: Sun Life Coverage API
  slug: sun-life-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-coverage-api-openapi.yml
- filename: sun-life-endpoint-api-openapi.yml
  format: yaml
  label: Sun Life Endpoint API
  slug: sun-life-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-endpoint-api-openapi.yml
- filename: sun-life-healthcareservice-api-openapi.yml
  format: yaml
  label: Sun Life Healthcare Service API
  slug: sun-life-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-healthcareservice-api-openapi.yml
- filename: sun-life-insuranceplan-api-openapi.yml
  format: yaml
  label: Sun Life Insurance Plan API
  slug: sun-life-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-insuranceplan-api-openapi.yml
- filename: sun-life-location-api-openapi.yml
  format: yaml
  label: Sun Life Location API
  slug: sun-life-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-location-api-openapi.yml
- filename: sun-life-metadata-api-openapi.yml
  format: yaml
  label: Sun Life Metadata API
  slug: sun-life-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-metadata-api-openapi.yml
- filename: sun-life-organization-api-openapi.yml
  format: yaml
  label: Sun Life Organization API
  slug: sun-life-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-organization-api-openapi.yml
- filename: sun-life-patient-api-openapi.yml
  format: yaml
  label: Sun Life Patient API
  slug: sun-life-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-patient-api-openapi.yml
- filename: sun-life-practitioner-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner API
  slug: sun-life-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitioner-api-openapi.yml
- filename: sun-life-practitionerrole-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner Role API
  slug: sun-life-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitionerrole-api-openapi.yml
- filename: sun-life-relatedperson-api-openapi.yml
  format: yaml
  label: Sun Life Related Person API
  slug: sun-life-relatedperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-relatedperson-api-openapi.yml
- filename: sun-life-token-api-openapi.yml
  format: yaml
  label: Sun Life Token API
  slug: sun-life-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-token-api-openapi.yml
- filename: sun-life-tokenhook-api-openapi.yml
  format: yaml
  label: Sun Life Tokenhook API
  slug: sun-life-tokenhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-tokenhook-api-openapi.yml
- filename: sun-life-well-known-api-openapi.yml
  format: yaml
  label: Sun Life .well Known API
  slug: sun-life-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-well-known-api-openapi.yml
authorization_urls:
- https://api.dentaquest.com/FhirPatientAccess/v1/authorize
description: ''
docs: https://www.dentaquest.com/en/interoperability-api
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sun Life Scopes
name_suffix: OAuth Scopes
note: SMART App Launch 1.0.0 scopes published by the DentaQuest FHIR Patient Access API (Sun Life U.S. dental).
overview: 'Sun Life publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sun Life API on a user''s behalf.


  Tokens are issued from https://api.dentaquest.com/FhirPatientAccess/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sun Life
provider_slug: sun-life
schemes:
- flows:
  - authorizationUrl: https://api.dentaquest.com/FhirPatientAccess/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.dentaquest.com/FhirPatientAccess/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.dentaquest.com/FhirPatientAccess/v1/token
  name: SMART on FHIR
  source: well-known/sun-life-dentaquest-smart-configuration.json
scope_count: 5
scope_names:
- patient/*.read
- launch/patient
- offline_access
- openid
- fhirUser
scopes:
- description: Read access to every FHIR resource in the authorized patient compartment (Patient, Coverage, Organization, Practitioner, RelatedPerson).
  flows:
  - authorizationCode
  scope: patient/*.read
- description: Request the standalone patient launch context so the app is bound to one member.
  flows:
  - authorizationCode
  scope: launch/patient
- description: Issue a refresh token so the app can keep reading after the member leaves the browser.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication; returns an id_token for the member.
  flows:
  - authorizationCode
  scope: openid
- description: Return the FHIR resource representing the authenticated user.
  flows:
  - authorizationCode
  scope: fhirUser
slug: sun-life-scopes
source_filename: sun-life-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://api.dentaquest.com/FhirPatientAccess/v1/.well-known/smart-configuration\ndocs: https://www.dentaquest.com/en/interoperability-api\nnote: SMART App Launch 1.0.0 scopes published by the DentaQuest FHIR Patient Access API (Sun Life U.S.\n  dental).\nschemes:\n- name: SMART on FHIR\n  source: well-known/sun-life-dentaquest-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.dentaquest.com/FhirPatientAccess/v1/authorize\n    tokenUrl: https://api.dentaquest.com/FhirPatientAccess/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.dentaquest.com/FhirPatientAccess/v1/token\nscopes:\n- scope: patient/*.read\n  description: Read access to every FHIR resource in the authorized patient compartment (Patient, Coverage,\n    Organization, Practitioner, RelatedPerson).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\n\
  - scope: launch/patient\n  description: Request the standalone patient launch context so the app is bound to one member.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\n- scope: offline_access\n  description: Issue a refresh token so the app can keep reading after the member leaves the browser.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token for the member.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\n- scope: fhirUser\n  description: Return the FHIR resource representing the authenticated user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\nauthorization_server_scopes:\n  issuer: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7\n  scopes_supported:\n  - interclient_access\n\
  \  - openid\n  - profile\n  - email\n  - address\n  - phone\n  - offline_access\n  - device_sso\n  source: well-known/sun-life-dentaquest-okta-openid-configuration.json\n  note: Okta authorization-server scopes; the FHIR-facing scope set published for app developers is the\n    SMART list above.\nnot_offered:\n- scope: user/*.read\n  note: Not advertised in smart-configuration despite permission-user in capabilities.\n- scope: '*.write'\n  note: The Patient Access API is read-only; no write scopes are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/scopes/sun-life-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Benefits
- Dental Insurance
- Disability
- Wealth Management
- Financial-Services
- Carrier
- FHIR
- Patient Access
- Provider Directory
- Healthcare Interoperability
- CMS-9115-F
- DentaQuest
- SMART on FHIR
- Dental Benefits
token_urls:
- https://api.dentaquest.com/FhirPatientAccess/v1/token
---
