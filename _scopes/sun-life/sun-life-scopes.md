---
api_specs:
- filename: sun-life-dentaquest-fhir-patient-access-openapi.json
  format: json
  label: DentaQuest FHIR Patient Access API
  slug: sun-life-dentaquest-fhir-patient-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-patient-access-openapi.json
- filename: sun-life-dentaquest-fhir-provider-directory-openapi.json
  format: json
  label: DentaQuest FHIR Provider Directory API
  slug: sun-life-dentaquest-fhir-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json
- filename: sun-life-dentaquest-fhir-metadata-openapi.json
  format: json
  label: DentaQuest FHIR Metadata API
  slug: sun-life-dentaquest-fhir-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-metadata-openapi.json
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
