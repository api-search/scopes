---
api_specs:
- filename: elation-allergies-api-openapi.yml
  format: yaml
  label: Elation Health Allergies API
  slug: elation-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-allergies-api-openapi.yml
- filename: elation-appointments-api-openapi.yml
  format: yaml
  label: Elation Health Appointments API
  slug: elation-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-appointments-api-openapi.yml
- filename: elation-authentication-api-openapi.yml
  format: yaml
  label: Elation Health Authentication API
  slug: elation-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-authentication-api-openapi.yml
- filename: elation-billing-api-openapi.yml
  format: yaml
  label: Elation Health Billing API
  slug: elation-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-billing-api-openapi.yml
- filename: elation-insurance-api-openapi.yml
  format: yaml
  label: Elation Health Insurance API
  slug: elation-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-insurance-api-openapi.yml
- filename: elation-lab-orders-api-openapi.yml
  format: yaml
  label: Elation Health Lab Orders API
  slug: elation-lab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-lab-orders-api-openapi.yml
- filename: elation-medications-api-openapi.yml
  format: yaml
  label: Elation Health Medications API
  slug: elation-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-medications-api-openapi.yml
- filename: elation-messaging-api-openapi.yml
  format: yaml
  label: Elation Health Messaging API
  slug: elation-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-messaging-api-openapi.yml
- filename: elation-patients-api-openapi.yml
  format: yaml
  label: Elation Health Patients API
  slug: elation-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-patients-api-openapi.yml
- filename: elation-physicians-api-openapi.yml
  format: yaml
  label: Elation Health Physicians API
  slug: elation-physicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-physicians-api-openapi.yml
- filename: elation-practices-api-openapi.yml
  format: yaml
  label: Elation Health Practices API
  slug: elation-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-practices-api-openapi.yml
- filename: elation-problems-api-openapi.yml
  format: yaml
  label: Elation Health Problems API
  slug: elation-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-problems-api-openapi.yml
- filename: elation-visit-notes-api-openapi.yml
  format: yaml
  label: Elation Health Visit Notes API
  slug: elation-visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-visit-notes-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Elation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elation Health publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elation Health API on a user''s behalf.


  Tokens are issued from https://sandbox.elationemr.com/api/2.0/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elation Health
provider_slug: elation
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-elation-health-api-openapi.yml
scope_count: 1
scope_names:
- apiv2
scopes:
- description: Full API access
  flows:
  - clientCredentials
  scope: apiv2
slug: elation-scopes
source_filename: elation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elation-elation-health-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/elation-elation-health-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.elationemr.com/api/2.0/oauth2/token/\nscopes:\n- scope: apiv2\n  description: Full API access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/elation-elation-health-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/scopes/elation-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- EHR
- Electronic Health Records
- Primary Care
- Healthcare
- FHIR
- Clinical
- Patients
- Prescriptions
- Messaging
token_urls:
- https://sandbox.elationemr.com/api/2.0/oauth2/token/
---
