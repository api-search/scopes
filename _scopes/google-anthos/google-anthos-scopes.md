---
api_specs:
- filename: gke-on-prem-api-openapi.yml
  format: yaml
  label: GKE On-Prem API
  slug: gke-on-prem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/openapi/gke-on-prem-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Anthos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Anthos publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Anthos API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Anthos
provider_slug: google-anthos
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/gke-on-prem-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Full access to Google Cloud resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-anthos-scopes
source_filename: google-anthos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gke-on-prem-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/gke-on-prem-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gke-on-prem-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/scopes/google-anthos-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Container Platform
- Hybrid Cloud
- Kubernetes
- Multi-Cloud
- On-Premises
- Service Mesh
token_urls:
- https://oauth2.googleapis.com/token
---
