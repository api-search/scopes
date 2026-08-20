---
api_specs:
- filename: diagnostic-robotics-precision-population-health-openapi.yml
  format: yaml
  label: Diagnostic Robotics Precision Population Health API
  slug: diagnostic-robotics-precision-population-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-precision-population-health-openapi.yml
- filename: diagnostic-robotics-patient-questionnaire-openapi.yml
  format: yaml
  label: Diagnostic Robotics Patient Questionnaire API
  slug: diagnostic-robotics-patient-questionnaire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-patient-questionnaire-openapi.yml
- filename: diagnostic-robotics-symptom-search-openapi.yml
  format: yaml
  label: Diagnostic Robotics Symptom Search Service
  slug: diagnostic-robotics-symptom-search-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-symptom-search-openapi.yml
authorization_urls:
- https://digital-outreach.us.auth0.com/authorize?audience=dev-digital-outreach-api-identifier
description: ''
docs: https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Diagnostic Robotics Scopes
name_suffix: OAuth Scopes
note: 'Both OAuth 2.0 schemes declare an EMPTY scopes map in the published OpenAPI, and the authentication guide documents no scopes, permissions or consent screen - a client_id/client_secret pair is exchanged for a bearer token that carries the full tenant grant. There is no published scope or permission reference page to search. Authorization is therefore tenant-scoped rather than scope-scoped: an agent holding a token can read patient risk profiles, patient demographics and HCC/RAF diagnosis data and can PATCH diagnoses, with no narrower grant available. Recorded as an honest zero, not a gap in harvesting.'
overview: 'Diagnostic Robotics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Diagnostic Robotics
provider_slug: diagnostic-robotics
schemes:
- flows:
  - flow: password
    tokenUrl: /api/oauth/token
  name: OAuth2PasswordBearer
  source: openapi/diagnostic-robotics-precision-population-health-openapi.yml
- flows:
  - authorizationUrl: https://digital-outreach.us.auth0.com/authorize?audience=dev-digital-outreach-api-identifier
    flow: authorizationCode
    tokenUrl: https://digital-outreach.us.auth0.com/oauth/token
  name: OAuth2AuthorizationCodeBearer
  source: openapi/diagnostic-robotics-precision-population-health-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: diagnostic-robotics-scopes
source_filename: diagnostic-robotics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/diagnostic-robotics-precision-population-health-openapi.yml\ndocs: https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/diagnostic-robotics-precision-population-health-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/oauth/token\n- name: OAuth2AuthorizationCodeBearer\n  source: openapi/diagnostic-robotics-precision-population-health-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://digital-outreach.us.auth0.com/authorize?audience=dev-digital-outreach-api-identifier\n    tokenUrl: https://digital-outreach.us.auth0.com/oauth/token\nscopes: []\nscope_count: 0\nnote: >-\n  Both OAuth 2.0 schemes declare an EMPTY scopes map in the published OpenAPI, and the authentication guide\n  documents no scopes, permissions or consent screen - a client_id/client_secret pair is exchanged\
  \ for a bearer\n  token that carries the full tenant grant. There is no published scope or permission reference page to search.\n  Authorization is therefore tenant-scoped rather than scope-scoped: an agent holding a token can read patient\n  risk profiles, patient demographics and HCC/RAF diagnosis data and can PATCH diagnoses, with no narrower grant\n  available. Recorded as an honest zero, not a gap in harvesting.\nsearched:\n  pages_checked:\n  - url: https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication\n    status: 200\n    result: no scope reference\n  - url: https://digital-outreach.us.auth0.com/.well-known/openid-configuration\n    status: 404\n    result: Auth0 tenant no longer resolves, so scopes_supported cannot be read from discovery\n  checked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/scopes/diagnostic-robotics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Health
- Healthcare
- Clinical AI
- Population Health
- Risk Adjustment
- Predictive Analytics
- triage
- FHIR
- Claims Data
- Care Management
- Payers
- Medical Coding
token_urls:
- /api/oauth/token
- https://digital-outreach.us.auth0.com/oauth/token
---
