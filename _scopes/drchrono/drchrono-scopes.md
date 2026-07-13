---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: drchrono REST API
  slug: drchrono-rest-api
  spec_type: OpenAPI
  url: https://app.drchrono.com/api-docs/
authorization_urls:
- https://app.drchrono.com/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Drchrono Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'drchrono publishes 23 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the drchrono API on a user''s behalf.


  Tokens are issued from https://app.drchrono.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: drchrono
provider_slug: drchrono
schemes:
- flows:
  - authorizationUrl: https://app.drchrono.com/o/authorize/
    flow: authorizationCode
    tokenUrl: https://app.drchrono.com/o/token/
  name: drchrono_oauth2
  source: openapi/drchrono-rest-api-openapi.yml
scope_count: 23
scope_names:
- billing
- billing:patient-payment:read
- billing:patient-payment:write
- billing:read
- billing:write
- calendar:read
- calendar:write
- clinical:read
- clinical:write
- labs:read
- labs:write
- messages:read
- messages:write
- patients:read
- patients:summary:read
- patients:summary:write
- patients:write
- settings:read
- settings:write
- tasks:read
- tasks:write
- user:read
- user:write
scopes:
- description: ''
  flows: []
  scope: billing
- description: View patient payment information
  flows:
  - authorizationCode
  scope: billing:patient-payment:read
- description: Modify patient payment information
  flows:
  - authorizationCode
  scope: billing:patient-payment:write
- description: View billing information.
  flows:
  - authorizationCode
  scope: billing:read
- description: Modify billing information.
  flows:
  - authorizationCode
  scope: billing:write
- description: View your appointments.
  flows:
  - authorizationCode
  scope: calendar:read
- description: Schedule appointments and modify the data associated with them.
  flows:
  - authorizationCode
  scope: calendar:write
- description: View clinical information, such as vitals, clinical notes, medications and diagnoses.
  flows:
  - authorizationCode
  scope: clinical:read
- description: Create and modify clinical information, such as vitals, clinical notes, medications and diagnoses.
  flows:
  - authorizationCode
  scope: clinical:write
- description: View patient lab orders and results.
  flows:
  - authorizationCode
  scope: labs:read
- description: Create and modify patient lab orders and results.
  flows:
  - authorizationCode
  scope: labs:write
- description: View messages in your message center.
  flows:
  - authorizationCode
  scope: messages:read
- description: Create and modify messages in your message center.
  flows:
  - authorizationCode
  scope: messages:write
- description: View detailed patient information.
  flows:
  - authorizationCode
  scope: patients:read
- description: View summary information about your patients. This includes patients' name, chart_id, age, and gender.
  flows:
  - authorizationCode
  scope: patients:summary:read
- description: Create new patients and set their name, chart_id, age, and gender.
  flows:
  - authorizationCode
  scope: patients:summary:write
- description: Create patients and modify detailed patient information.
  flows:
  - authorizationCode
  scope: patients:write
- description: View resources that requires Settings permission, such as custom fields.
  flows:
  - authorizationCode
  scope: settings:read
- description: Create resources that requires Settings permission, such as custom fields.
  flows:
  - authorizationCode
  scope: settings:write
- description: View tasks in your tasks center
  flows:
  - authorizationCode
  scope: tasks:read
- description: Create and modify tasks in your tasks center
  flows:
  - authorizationCode
  scope: tasks:write
- description: View your basic information.
  flows:
  - authorizationCode
  scope: user:read
- description: Edit select account information, such as creating new exam rooms.
  flows:
  - authorizationCode
  scope: user:write
slug: drchrono-scopes
source_filename: drchrono-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drchrono-rest-api-openapi.yml\nschemes:\n- name: drchrono_oauth2\n  source: openapi/drchrono-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.drchrono.com/o/authorize/\n    tokenUrl: https://app.drchrono.com/o/token/\nscopes:\n- scope: billing\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: billing:patient-payment:read\n  description: View patient payment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: billing:patient-payment:write\n  description: Modify patient payment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: billing:read\n  description: View billing information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: billing:write\n  description: Modify billing information.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: calendar:read\n  description: View your appointments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: calendar:write\n  description: Schedule appointments and modify the data associated with them.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: clinical:read\n  description: View clinical information, such as vitals, clinical notes, medications and diagnoses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: clinical:write\n  description: Create and modify clinical information, such as vitals, clinical notes, medications\n    and diagnoses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: labs:read\n  description: View patient lab orders and results.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n\
  - scope: labs:write\n  description: Create and modify patient lab orders and results.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: messages:read\n  description: View messages in your message center.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: messages:write\n  description: Create and modify messages in your message center.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: patients:read\n  description: View detailed patient information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: patients:summary:read\n  description: View summary information about your patients. This includes patients' name, chart_id,\n    age, and gender.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: patients:summary:write\n  description: Create new patients and\
  \ set their name, chart_id, age, and gender.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: patients:write\n  description: Create patients and modify detailed patient information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: settings:read\n  description: View resources that requires Settings permission, such as custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: settings:write\n  description: Create resources that requires Settings permission, such as custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: tasks:read\n  description: View tasks in your tasks center\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: tasks:write\n  description: Create and modify tasks in your tasks center\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: user:read\n  description: View your basic information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n- scope: user:write\n  description: Edit select account information, such as creating new exam rooms.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drchrono-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/scopes/drchrono-scopes.yml
summary_line: 23 scopes · authorizationCode
tags:
- EHR
- Electronic Health Records
- Healthcare
- Medical Records
- Practice Management
- HIPAA
- Appointments
- Billing
- Prescriptions
- Lab Integration
- FHIR
token_urls:
- https://app.drchrono.com/o/token/
---
