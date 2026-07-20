---
api_specs:
- filename: clever-care-coverage-openapi.json
  format: json
  label: Clever Care FHIR Coverage
  slug: clever-care-fhir-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-coverage-openapi.json
- filename: clever-care-endpoint-openapi.json
  format: json
  label: Clever Care FHIR Endpoint
  slug: clever-care-fhir-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-endpoint-openapi.json
- filename: clever-care-explanation-of-benefit-openapi.json
  format: json
  label: Clever Care FHIR ExplanationOfBenefit
  slug: clever-care-fhir-explanationofbenefit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-explanation-of-benefit-openapi.json
- filename: clever-care-healthcare-service-openapi.json
  format: json
  label: Clever Care FHIR HealthcareService
  slug: clever-care-fhir-healthcareservice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-healthcare-service-openapi.json
- filename: clever-care-insurance-plan-openapi.json
  format: json
  label: Clever Care FHIR InsurancePlan
  slug: clever-care-fhir-insuranceplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-insurance-plan-openapi.json
- filename: clever-care-list-openapi.json
  format: json
  label: Clever Care FHIR List
  slug: clever-care-fhir-list
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-list-openapi.json
- filename: clever-care-location-openapi.json
  format: json
  label: Clever Care FHIR Location
  slug: clever-care-fhir-location
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-location-openapi.json
- filename: clever-care-medication-knowledge-openapi.json
  format: json
  label: Clever Care FHIR MedicationKnowledge
  slug: clever-care-fhir-medicationknowledge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-medication-knowledge-openapi.json
- filename: clever-care-organization-openapi.json
  format: json
  label: Clever Care FHIR Organization
  slug: clever-care-fhir-organization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-openapi.json
- filename: clever-care-organization-affiliation-openapi.json
  format: json
  label: Clever Care FHIR OrganizationAffiliation
  slug: clever-care-fhir-organizationaffiliation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-affiliation-openapi.json
- filename: clever-care-patient-openapi.json
  format: json
  label: Clever Care FHIR Patient
  slug: clever-care-fhir-patient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-patient-openapi.json
- filename: clever-care-practitioner-openapi.json
  format: json
  label: Clever Care FHIR Practitioner
  slug: clever-care-fhir-practitioner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-openapi.json
- filename: clever-care-practitioner-role-openapi.json
  format: json
  label: Clever Care FHIR PractitionerRole
  slug: clever-care-fhir-practitionerrole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-role-openapi.json
authorization_urls: []
description: ''
docs: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clever Care Scopes
name_suffix: OAuth Scopes
note: Clever Care exposes SMART on FHIR (SMART App Launch) scopes for its secured Patient Access resources (Patient, ExplanationOfBenefit, Coverage). The OpenAPI securityDefinitions carry an empty scope map (WSO2 gateway default); the authoritative scope list comes from the published SMART configuration document at /r4/.well-known/smart-configuration.
overview: 'Clever Care publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clever Care API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clever Care
provider_slug: clever-care
schemes:
- authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize
  grantTypes:
  - authorization_code
  - client_credentials
  jwksUri: https://fhir-portal.clevercarehealthplan.com/oauth2/jwks
  name: SMART on FHIR (OAuth 2.0 / OpenID Connect)
  pkce: S256
  revocationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/revoke
  sources:
  - openapi/clever-care-patient-openapi.json
  - openapi/clever-care-explanation-of-benefit-openapi.json
  - openapi/clever-care-coverage-openapi.json
  tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
scope_count: 4
scope_names:
- openid
- launch/patient
- patient/*.cruds
- user/*.cruds
scopes:
- description: OpenID Connect authentication; returns an id_token identifying the member.
  flows:
  - authorization_code
  scope: openid
- description: Standalone patient launch context; binds the access token to a single patient/member.
  flows:
  - authorization_code
  scope: launch/patient
- description: Patient-level access to all authorized FHIR resource types (CARIN BB Patient, ExplanationOfBenefit, Coverage) for the launched patient. SMART v2 granular scope; 'cruds' = create/read/update/delete/search (Clever Care exposes read+search).
  flows:
  - authorization_code
  scope: patient/*.cruds
- description: User-level access to all authorized FHIR resource types the authenticated user is permitted to see. SMART v2 granular scope.
  flows:
  - authorization_code
  scope: user/*.cruds
slug: clever-care-scopes
source_filename: clever-care-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi securityDefinitions (13 FHIR resource APIs)\ndocs: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration\nsmart_configuration: well-known/clever-care-smart-configuration.json\nnote: >-\n  Clever Care exposes SMART on FHIR (SMART App Launch) scopes for its secured\n  Patient Access resources (Patient, ExplanationOfBenefit, Coverage). The\n  OpenAPI securityDefinitions carry an empty scope map (WSO2 gateway default);\n  the authoritative scope list comes from the published SMART configuration\n  document at /r4/.well-known/smart-configuration.\nschemes:\n- name: SMART on FHIR (OAuth 2.0 / OpenID Connect)\n  authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize\n  tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n  jwksUri: https://fhir-portal.clevercarehealthplan.com/oauth2/jwks\n  revocationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/revoke\n\
  \  grantTypes: [authorization_code, client_credentials]\n  pkce: S256\n  sources:\n  - openapi/clever-care-patient-openapi.json\n  - openapi/clever-care-explanation-of-benefit-openapi.json\n  - openapi/clever-care-coverage-openapi.json\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token identifying the member.\n  flows: [authorization_code]\n- scope: launch/patient\n  description: Standalone patient launch context; binds the access token to a single patient/member.\n  flows: [authorization_code]\n- scope: patient/*.cruds\n  description: >-\n    Patient-level access to all authorized FHIR resource types (CARIN BB Patient,\n    ExplanationOfBenefit, Coverage) for the launched patient. SMART v2 granular\n    scope; 'cruds' = create/read/update/delete/search (Clever Care exposes read+search).\n  flows: [authorization_code]\n- scope: user/*.cruds\n  description: >-\n    User-level access to all authorized FHIR resource types the authenticated user\n\
  \    is permitted to see. SMART v2 granular scope.\n  flows: [authorization_code]\nsmart_capabilities:\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- context-standalone-patient\n- sso-openid-connect\n- permission-patient\n- permission-offline\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/scopes/clever-care-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Life Sciences
- Health Insurance
- Medicare Advantage
- Healthcare
- FHIR
- Healthcare Interoperability
- Patient Access
- Provider Directory
- CMS-9115-F
token_urls: []
---
