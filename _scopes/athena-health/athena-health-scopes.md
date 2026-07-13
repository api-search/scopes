---
api_specs:
- filename: athenahealth-athenaone-rest-api-openapi.yml
  format: yaml
  label: athenahealth athenaOne REST API
  slug: athenahealth-athenaone-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-athenaone-rest-api-openapi.yml
- filename: athenahealth-fhir-r4-api-openapi.yml
  format: yaml
  label: athenahealth FHIR R4 API
  slug: athenahealth-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-r4-api-openapi.yml
- filename: athenahealth-fhir-subscriptions-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Subscriptions API
  slug: athenahealth-fhir-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-subscriptions-api-openapi.yml
- filename: athenahealth-fhir-bulk-data-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Bulk Data Access API
  slug: athenahealth-fhir-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-bulk-data-api-openapi.yml
- filename: athenahealth-cds-hooks-api-openapi.yml
  format: yaml
  label: athenahealth CDS Hooks API
  slug: athenahealth-cds-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-cds-hooks-api-openapi.yml
authorization_urls:
- https://api.platform.athenahealth.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Athena Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'athenahealth publishes 11 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the athenahealth API on a user''s behalf.


  Tokens are issued from https://api.platform.athenahealth.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: athenahealth
provider_slug: athena-health
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  - authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: oauth2
  source: openapi/athenahealth-athenaone-rest-api-openapi.yml
- description: SMART Backend Services (JWT client assertion)
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: backend
  source: openapi/athenahealth-fhir-bulk-data-api-openapi.yml
- description: SMART on FHIR / OAuth 2.0
  flows:
  - authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: smart
  source: openapi/athenahealth-fhir-r4-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token
  name: oauth2
  source: openapi/athenahealth-fhir-subscriptions-api-openapi.yml
scope_count: 11
scope_names:
- athena/service/Athenanet.MDP.*
- fhirUser
- launch
- launch/patient
- offline_access
- openid
- patient/*.read
- system/*.read
- system/Subscription.read
- system/Subscription.write
- user/*.read
scopes:
- description: athenahealth MDP scope
  flows:
  - authorizationCode
  - clientCredentials
  scope: athena/service/Athenanet.MDP.*
- description: Current FHIR user identity
  flows:
  - authorizationCode
  scope: fhirUser
- description: SMART launch context
  flows:
  - authorizationCode
  scope: launch
- description: Patient launch context
  flows:
  - authorizationCode
  scope: launch/patient
- description: Issue refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Read patient-scoped resources
  flows:
  - authorizationCode
  scope: patient/*.read
- description: System-level read for Bulk Data
  flows:
  - authorizationCode
  - clientCredentials
  scope: system/*.read
- description: Read Subscriptions
  flows:
  - clientCredentials
  scope: system/Subscription.read
- description: Manage Subscriptions
  flows:
  - clientCredentials
  scope: system/Subscription.write
- description: Read user-scoped resources
  flows:
  - authorizationCode
  scope: user/*.read
slug: athena-health-scopes
source_filename: athena-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/athenahealth-athenaone-rest-api-openapi.yml, openapi/athenahealth-fhir-bulk-data-api-openapi.yml,\n  openapi/athenahealth-fhir-r4-api-openapi.yml, openapi/athenahealth-fhir-subscriptions-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/athenahealth-athenaone-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n- name: backend\n  source: openapi/athenahealth-fhir-bulk-data-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n  description: SMART Backend Services (JWT client assertion)\n- name: smart\n  source: openapi/athenahealth-fhir-r4-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://api.platform.athenahealth.com/oauth2/v1/authorize\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\n  description: SMART on FHIR / OAuth 2.0\n- name: oauth2\n  source: openapi/athenahealth-fhir-subscriptions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.platform.athenahealth.com/oauth2/v1/token\nscopes:\n- scope: athena/service/Athenanet.MDP.*\n  description: athenahealth MDP scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/athenahealth-athenaone-rest-api-openapi.yml\n- scope: fhirUser\n  description: Current FHIR user identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: launch\n  description: SMART launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n\
  - scope: launch/patient\n  description: Patient launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: offline_access\n  description: Issue refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: patient/*.read\n  description: Read patient-scoped resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: system/*.read\n  description: System-level read for Bulk Data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/athenahealth-fhir-bulk-data-api-openapi.yml\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n- scope: system/Subscription.read\n  description: Read Subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/athenahealth-fhir-subscriptions-api-openapi.yml\n\
  - scope: system/Subscription.write\n  description: Manage Subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/athenahealth-fhir-subscriptions-api-openapi.yml\n- scope: user/*.read\n  description: Read user-scoped resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/athenahealth-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/scopes/athena-health-scopes.yml
summary_line: 11 scopes · clientCredentials/authorizationCode
tags:
- EHR
- Electronic Health Records
- Healthcare
- HL7
- FHIR
- Interoperability
- Practice Management
- Revenue Cycle Management
- USCDI
- Cures Act
- SMART on FHIR
- CDS Hooks
- Cloud EHR
token_urls:
- https://api.platform.athenahealth.com/oauth2/v1/token
---
