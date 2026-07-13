---
api_specs:
- filename: llms.txt
  format: yaml
  label: Elation Health REST API
  slug: elation-health-api
  spec_type: OpenAPI
  url: https://docs.elationhealth.com/llms.txt
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
