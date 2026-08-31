---
api_specs:
- filename: metabolon-assistant-api-openapi.yml
  format: yaml
  label: Metabolon Assistant API
  slug: metabolon-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-assistant-api-openapi.yml
- filename: metabolon-auth-api-openapi.yml
  format: yaml
  label: Metabolon Auth API
  slug: metabolon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-auth-api-openapi.yml
- filename: metabolon-decentralization-api-openapi.yml
  format: yaml
  label: Metabolon Decentralization API
  slug: metabolon-decentralization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-decentralization-api-openapi.yml
- filename: metabolon-eula-api-openapi.yml
  format: yaml
  label: Metabolon Eula API
  slug: metabolon-eula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-eula-api-openapi.yml
- filename: metabolon-files-api-openapi.yml
  format: yaml
  label: Metabolon Files API
  slug: metabolon-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-files-api-openapi.yml
- filename: metabolon-health-api-openapi.yml
  format: yaml
  label: Metabolon Health API
  slug: metabolon-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-health-api-openapi.yml
- filename: metabolon-labvantagefiles-api-openapi.yml
  format: yaml
  label: Metabolon Lab Vantage Files API
  slug: metabolon-labvantagefiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-labvantagefiles-api-openapi.yml
- filename: metabolon-pipelinestatus-api-openapi.yml
  format: yaml
  label: Metabolon Pipeline Status API
  slug: metabolon-pipelinestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-pipelinestatus-api-openapi.yml
- filename: metabolon-projects-api-openapi.yml
  format: yaml
  label: Metabolon Projects API
  slug: metabolon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-projects-api-openapi.yml
- filename: metabolon-reports-api-openapi.yml
  format: yaml
  label: Metabolon Reports API
  slug: metabolon-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-reports-api-openapi.yml
- filename: metabolon-samplesets-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets API
  slug: metabolon-samplesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesets-api-openapi.yml
- filename: metabolon-samplesetsinfo-api-openapi.yml
  format: yaml
  label: Metabolon Sample Sets Info API
  slug: metabolon-samplesetsinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-samplesetsinfo-api-openapi.yml
- filename: metabolon-search-api-openapi.yml
  format: yaml
  label: Metabolon Search API
  slug: metabolon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-search-api-openapi.yml
- filename: metabolon-sharedfile-api-openapi.yml
  format: yaml
  label: Metabolon Shared File API
  slug: metabolon-sharedfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-sharedfile-api-openapi.yml
- filename: metabolon-spectraldata-api-openapi.yml
  format: yaml
  label: Metabolon Spectral Data API
  slug: metabolon-spectraldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-spectraldata-api-openapi.yml
- filename: metabolon-status-api-openapi.yml
  format: yaml
  label: Metabolon Status API
  slug: metabolon-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-status-api-openapi.yml
- filename: metabolon-studybuilder-api-openapi.yml
  format: yaml
  label: Metabolon Study Builder API
  slug: metabolon-studybuilder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-studybuilder-api-openapi.yml
- filename: metabolon-users-api-openapi.yml
  format: yaml
  label: Metabolon Users API
  slug: metabolon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Metabolon Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found zero oauth2 securitySchemes because none of the four published Metabolon OpenAPI documents declares any security at all. The scopes below are the scopes_supported list advertised by Metabolon's own Auth0 tenant discovery document — they are the stock OIDC identity scopes and none of them is an API authorization scope. Metabolon publishes no scopes or permissions reference page. API authorization is done with server-side roles and per-project entitlements instead (see authentication/metabolon-authentication.yml#authorization), so there is no scope-to-operation mapping to record and none has been invented.
overview: 'Metabolon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Metabolon
provider_slug: metabolon
schemes:
- authorization_url: https://auth0.metabolon.com/authorize
  issuer: https://auth0.metabolon.com/
  name: Auth0 OIDC
  source: well-known/metabolon-openid-configuration.json
  token_url: https://auth0.metabolon.com/oauth/token
  type: openIdConnect
scope_count: 0
scope_names: []
scopes: []
slug: metabolon-scopes
source_filename: metabolon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://auth0.metabolon.com/.well-known/openid-configuration\nnote: >-\n  derive-oauth-scopes.py found zero oauth2 securitySchemes because none of the four published Metabolon\n  OpenAPI documents declares any security at all. The scopes below are the scopes_supported list advertised\n  by Metabolon's own Auth0 tenant discovery document — they are the stock OIDC identity scopes and none of\n  them is an API authorization scope. Metabolon publishes no scopes or permissions reference page. API\n  authorization is done with server-side roles and per-project entitlements instead (see\n  authentication/metabolon-authentication.yml#authorization), so there is no scope-to-operation mapping to\n  record and none has been invented.\ndocs: null\nauthorization_model: role-and-project entitlement, not scope-based\nschemes:\n- name: Auth0 OIDC\n  type: openIdConnect\n  issuer: https://auth0.metabolon.com/\n  authorization_url: https://auth0.metabolon.com/authorize\n\
  \  token_url: https://auth0.metabolon.com/oauth/token\n  source: well-known/metabolon-openid-configuration.json\nscope_count: 14\napi_scope_count: 0\nscopes:\n- name: openid\n  kind: oidc\n  description: Request an ID token (OIDC core).\n- name: profile\n  kind: oidc\n  description: Basic profile claims.\n- name: offline_access\n  kind: oidc\n  description: Issue a refresh token.\n- name: name\n  kind: oidc-claim\n- name: given_name\n  kind: oidc-claim\n- name: family_name\n  kind: oidc-claim\n- name: nickname\n  kind: oidc-claim\n- name: email\n  kind: oidc-claim\n- name: email_verified\n  kind: oidc-claim\n- name: picture\n  kind: oidc-claim\n- name: created_at\n  kind: oidc-claim\n- name: identities\n  kind: oidc-claim\n- name: phone\n  kind: oidc-claim\n- name: address\n  kind: oidc-claim\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/scopes/metabolon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Metabolomics
- Life Sciences
- Bioinformatics
- Multiomics
- Biotechnology
- Drug Discovery
- Precision Medicine
- Microbiome
- Biomarkers
- Contract Research
- Laboratory
token_urls: []
---
