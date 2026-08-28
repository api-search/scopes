---
api_specs:
- filename: metabolon-portal-api-openapi.yml
  format: yaml
  label: Metabolon Portal API
  slug: metabolon-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-portal-api-openapi.yml
- filename: metabolon-discovery-panels-api-openapi.yml
  format: yaml
  label: Metabolon Discovery Panels API
  slug: metabolon-discovery-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-discovery-panels-api-openapi.yml
- filename: metabolon-pathway-explorer-api-openapi.yml
  format: yaml
  label: Metabolon Pathway Explorer API
  slug: metabolon-pathway-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-pathway-explorer-api-openapi.yml
- filename: metabolon-heatmap-api-openapi.yml
  format: yaml
  label: Metabolon Heatmap API
  slug: metabolon-heatmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabolon/refs/heads/main/openapi/metabolon-heatmap-api-openapi.yml
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
