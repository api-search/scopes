---
api_specs:
- filename: drchrono-administrative-api-openapi.yml
  format: yaml
  label: drchrono Administrative API
  slug: drchrono-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-administrative-api-openapi.yml
- filename: drchrono-audit-api-openapi.yml
  format: yaml
  label: drchrono Audit API
  slug: drchrono-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-audit-api-openapi.yml
- filename: drchrono-availability-api-openapi.yml
  format: yaml
  label: drchrono Availability API
  slug: drchrono-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-availability-api-openapi.yml
- filename: drchrono-billing-api-openapi.yml
  format: yaml
  label: drchrono Billing API
  slug: drchrono-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-billing-api-openapi.yml
- filename: drchrono-clinical-api-openapi.yml
  format: yaml
  label: drchrono Clinical API
  slug: drchrono-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-clinical-api-openapi.yml
- filename: drchrono-practice-management-api-openapi.yml
  format: yaml
  label: drchrono Practice Management API
  slug: drchrono-practice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-practice-management-api-openapi.yml
authorization_urls:
- https://app.drchrono.com/o/authorize/
description: The 22 OAuth 2.0 scopes DrChrono declares on the drchrono_oauth2 security scheme of the OpenAPI it serves at https://app.drchrono.com/openapi-schema, with the scope-model narrative from the Authorization section of its API reference. Scopes take the form BASE_SCOPE:[read|write] over the bases user, calendar, patients, patients:summary, billing, clinical and labs, plus messages, tasks, settings and billing:patient-payment.
docs: https://app.drchrono.com/api-docs/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
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
  revocationUrl: https://app.drchrono.com/o/revoke_token
  source: openapi/_original/drchrono-rest-api-openapi-schema.json
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
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://app.drchrono.com/api-docs/\ndocs: https://app.drchrono.com/api-docs/\nname: drchrono REST v4 OAuth Scopes\ndescription: The 22 OAuth 2.0 scopes DrChrono declares on the drchrono_oauth2 security scheme of the OpenAPI it\n  serves at https://app.drchrono.com/openapi-schema, with the scope-model narrative from the Authorization section\n  of its API reference. Scopes take the form BASE_SCOPE:[read|write] over the bases user, calendar, patients, patients:summary,\n  billing, clinical and labs, plus messages, tasks, settings and billing:patient-payment.\nscope_count: 23\ndefault_behaviour: Omitting the scope parameter on the authorize call requests ALL scopes. DrChrono advises requesting\n  only the scopes an application needs.\npermission_gate: An OAuth scope is necessary but not sufficient. Each endpoint also requires an in-app permission\n  granted by a primary user inside the DrChrono web app; a correctly scoped token\
  \ returns 403 without it. The API\n  reference names the required scope AND permission per endpoint.\ngranularity_note: patients:summary is deliberately narrower than patients — it exposes only name, chart_id, age\n  and gender. DrChrono gives the example of a birthday-email application that should request patients:summary:read\n  rather than patients:read. Prefer the summary scope wherever identity is all you need; it is the minimum-necessary\n  posture the HIPAA obligations in the API terms call for.\nseparate_fhir_vocabulary: The SMART on FHIR R4 surface uses an entirely different scope vocabulary (233 SMART scopes)\n  against a different authorization server. See scopes/drchrono-fhir-smart-scopes.yml.\nschemes:\n- name: drchrono_oauth2\n  source: openapi/_original/drchrono-rest-api-openapi-schema.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.drchrono.com/o/authorize/\n    tokenUrl: https://app.drchrono.com/o/token/\n  revocationUrl: https://app.drchrono.com/o/revoke_token\n\
  scopes:\n- scope: billing\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: billing:patient-payment:read\n  description: View patient payment information\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: billing:patient-payment:write\n  description: Modify patient payment information\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: billing:read\n  description: View billing information.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: billing:write\n  description: Modify billing information.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n\
  - scope: calendar:read\n  description: View your appointments.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: calendar:write\n  description: Schedule appointments and modify the data associated with them.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: clinical:read\n  description: View clinical information, such as vitals, clinical notes, medications and diagnoses.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: clinical:write\n  description: Create and modify clinical information, such as vitals, clinical notes, medications and diagnoses.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n\
  - scope: labs:read\n  description: View patient lab orders and results.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: labs:write\n  description: Create and modify patient lab orders and results.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: messages:read\n  description: View messages in your message center.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: messages:write\n  description: Create and modify messages in your message center.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: patients:read\n  description: View detailed patient information.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: patients:summary:read\n  description: View summary information about your patients. This includes patients' name, chart_id, age, and gender.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: patients:summary:write\n  description: Create new patients and set their name, chart_id, age, and gender.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: patients:write\n  description: Create patients and modify detailed patient information.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: settings:read\n  description: View resources that requires\
  \ Settings permission, such as custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: settings:write\n  description: Create resources that requires Settings permission, such as custom fields.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: tasks:read\n  description: View tasks in your tasks center\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: tasks:write\n  description: Create and modify tasks in your tasks center\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: user:read\n  description: View your basic information.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n- scope: user:write\n  description: Edit select account information, such as creating new exam rooms.\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.drchrono.com/api-docs/\n  - openapi/_original/drchrono-rest-api-openapi-schema.json\n"
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
- SMART on FHIR
- USCDI
- Interoperability
- Webhook
- Authentication
- ONC Certified
- Telehealth
- Revenue Cycle Management
token_urls:
- https://app.drchrono.com/o/token/
---
