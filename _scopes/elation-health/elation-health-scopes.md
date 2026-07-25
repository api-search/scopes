---
api_specs:
- filename: elation-api-authentication.json
  format: json
  label: Elation OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-authentication.json
- filename: elation-patient-profile-api.json
  format: json
  label: Elation Patient Profile API
  slug: patient-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-profile-api.json
- filename: elation-visit-notes-api.json
  format: json
  label: Elation Visit Notes API
  slug: visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-visit-notes-api.json
- filename: elation-patient-document-api.json
  format: json
  label: Elation Patient Document API
  slug: patient-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-document-api.json
- filename: elation-orders-api.json
  format: json
  label: Elation Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-orders-api.json
- filename: elation-scheduling-api.json
  format: json
  label: Elation Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-scheduling-api.json
- filename: elation-billing-api.json
  format: json
  label: Elation Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-billing-api.json
- filename: elation-insurance-api.json
  format: json
  label: Elation Insurance API
  slug: insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-insurance-api.json
- filename: elation-premium-patient-insurance-api.json
  format: json
  label: Elation Patient Insurance API (Premium) & Eligibility
  slug: patient-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-premium-patient-insurance-api.json
- filename: elation-practice-api.json
  format: json
  label: Elation Practice API
  slug: practice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-practice-api.json
- filename: elation-user-management-api.json
  format: json
  label: Elation User Management API
  slug: user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-user-management-api.json
- filename: elation-messaging-api.json
  format: json
  label: Elation Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-messaging-api.json
- filename: elation-event-subscription-api.json
  format: json
  label: Elation Event Subscription API
  slug: event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-event-subscription-api.json
- filename: elation-reference-data-api.json
  format: json
  label: Elation Reference Data API
  slug: reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-reference-data-api.json
- filename: elation-care-gaps-api-1.json
  format: json
  label: Elation Care Gaps API
  slug: care-gaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-care-gaps-api-1.json
- filename: elation-elation-import-api.json
  format: json
  label: Elation Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-elation-import-api.json
authorization_urls: []
description: ''
docs: https://docs.elationhealth.com/reference/scopes
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: searched
name: Elation Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elation Health publishes 5 OAuth 2.0 scopes via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elation Health API on a user''s behalf.


  Tokens are issued from https://example.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elation Health
provider_slug: elation-health
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/elation-api-settings.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-billing-api.json
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/elation-care-gaps-api-1.json
- flows:
  - flow: password
    tokenUrl: http://www.elationhealth.com/api/2.0/oauth
  name: elation_auth
  source: openapi/elation-elation-import-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-event-subscription-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-insurance-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-messaging-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-orders-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-patient-document-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-patient-profile-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-practice-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-premium-patient-insurance-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-reference-data-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-scheduling-api.json
- flows:
  - flow: clientCredentials
    tokenUrl: /api/2.0/oauth2/token/
  name: oauth2
  source: openapi/elation-user-management-api.json
scope_count: 5
scope_names:
- act_as_user
- apiv2
- import
- system/{resource_name}.read
- system/{resource_name}.write
scopes:
- description: Impersonate a provider via X-On-Behalf-Of (combinable with apiv2 or system scopes)
  flows:
  - clientCredentials
  scope: act_as_user
- description: Full access to the API
  flows:
  - clientCredentials
  scope: apiv2
- description: interact with data imports in your practice
  flows:
  - password
  scope: import
- description: Read access to a specific resource
  flows:
  - clientCredentials
  scope: system/{resource_name}.read
- description: Write access to a specific resource
  flows:
  - clientCredentials
  scope: system/{resource_name}.write
slug: elation-health-scopes
source_filename: elation-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\ndocs: https://docs.elationhealth.com/reference/scopes\ndocs_note: >-\n  Confirmed against the published Token Scopes reference. Elation's OAuth2\n  client_credentials scopes are apiv2 (full access), act_as_user (provider\n  impersonation via X-On-Behalf-Of), and the granular system/{resource_name}.read\n  and system/{resource_name}.write pair. The legacy password-grant import scope\n  is used only by the Import API.\nsource: openapi/elation-api-settings.json, openapi/elation-billing-api.json, openapi/elation-care-gaps-api-1.json,\n  openapi/elation-elation-import-api.json, openapi/elation-event-subscription-api.json, openapi/elation-insurance-api.json,\n  openapi/elation-messaging-api.json, openapi/elation-orders-api.json, openapi/elation-patient-document-api.json,\n  openapi/elation-patient-profile-api.json, openapi/elation-practice-api.json, openapi/elation-premium-patient-insurance-api.json,\n  openapi/elation-reference-data-api.json,\
  \ openapi/elation-scheduling-api.json, openapi/elation-user-management-api.json\nschemes:\n- name: sec0\n  source: openapi/elation-api-settings.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: oauth2\n  source: openapi/elation-billing-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: OAuth2PasswordBearer\n  source: openapi/elation-care-gaps-api-1.json\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: elation_auth\n  source: openapi/elation-elation-import-api.json\n  flows:\n  - flow: password\n    tokenUrl: http://www.elationhealth.com/api/2.0/oauth\n- name: oauth2\n  source: openapi/elation-event-subscription-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-insurance-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-messaging-api.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-orders-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-patient-document-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-patient-profile-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-practice-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-premium-patient-insurance-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-reference-data-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-scheduling-api.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\n- name: oauth2\n  source: openapi/elation-user-management-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/2.0/oauth2/token/\nscopes:\n- scope: act_as_user\n  description: Impersonate a provider via X-On-Behalf-Of (combinable with apiv2 or system scopes)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/elation-billing-api.json\n  - openapi/elation-event-subscription-api.json\n  - openapi/elation-insurance-api.json\n  - openapi/elation-messaging-api.json\n  - openapi/elation-orders-api.json\n  - openapi/elation-patient-document-api.json\n  - openapi/elation-patient-profile-api.json\n  - openapi/elation-practice-api.json\n  - openapi/elation-premium-patient-insurance-api.json\n  - openapi/elation-reference-data-api.json\n  - openapi/elation-scheduling-api.json\n  - openapi/elation-user-management-api.json\n- scope: apiv2\n  description: Full access to the API\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/elation-billing-api.json\n  - openapi/elation-event-subscription-api.json\n  - openapi/elation-insurance-api.json\n  - openapi/elation-messaging-api.json\n  - openapi/elation-orders-api.json\n  - openapi/elation-patient-document-api.json\n  - openapi/elation-patient-profile-api.json\n  - openapi/elation-practice-api.json\n  - openapi/elation-premium-patient-insurance-api.json\n  - openapi/elation-reference-data-api.json\n  - openapi/elation-scheduling-api.json\n  - openapi/elation-user-management-api.json\n- scope: import\n  description: interact with data imports in your practice\n  flows:\n  - password\n  sources:\n  - openapi/elation-elation-import-api.json\n- scope: system/{resource_name}.read\n  description: Read access to a specific resource\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/elation-billing-api.json\n  - openapi/elation-event-subscription-api.json\n  - openapi/elation-insurance-api.json\n  - openapi/elation-messaging-api.json\n  -\
  \ openapi/elation-orders-api.json\n  - openapi/elation-patient-document-api.json\n  - openapi/elation-patient-profile-api.json\n  - openapi/elation-practice-api.json\n  - openapi/elation-premium-patient-insurance-api.json\n  - openapi/elation-reference-data-api.json\n  - openapi/elation-scheduling-api.json\n  - openapi/elation-user-management-api.json\n- scope: system/{resource_name}.write\n  description: Write access to a specific resource\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/elation-billing-api.json\n  - openapi/elation-event-subscription-api.json\n  - openapi/elation-insurance-api.json\n  - openapi/elation-messaging-api.json\n  - openapi/elation-orders-api.json\n  - openapi/elation-patient-document-api.json\n  - openapi/elation-patient-profile-api.json\n  - openapi/elation-practice-api.json\n  - openapi/elation-premium-patient-insurance-api.json\n  - openapi/elation-reference-data-api.json\n  - openapi/elation-scheduling-api.json\n  - openapi/elation-user-management-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/scopes/elation-health-scopes.yml
summary_line: 5 scopes · clientCredentials/password
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Primary Care
- Value-Based Care
- Eligibility
- Clinical Data
- Scheduling
- e-Prescribing
- Digital Health
token_urls:
- https://example.com/oauth2/token
- /api/2.0/oauth2/token/
- token
- http://www.elationhealth.com/api/2.0/oauth
---
