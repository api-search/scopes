---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Availity Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'availity publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the availity API on a user''s behalf.


  Tokens are issued from https://api.availity.com/availity/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: availity
provider_slug: availity
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.availity.com/availity/v1/token
  name: oauth2
  source: openapi/availity-claim-attachments-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.availity.com/availity/v1/token
  name: oauth2
  source: openapi/availity-claim-status-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.availity.com/availity/v1/token
  name: oauth2
  source: openapi/availity-eligibility-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.availity.com/availity/v1/token
  name: oauth2
  source: openapi/availity-service-reviews-openapi.yml
scope_count: 1
scope_names:
- hipaa
scopes:
- description: Access to HIPAA transaction APIs
  flows:
  - clientCredentials
  scope: hipaa
slug: availity-scopes
source_filename: availity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/availity-claim-attachments-openapi.yml, openapi/availity-claim-status-openapi.yml,\n  openapi/availity-eligibility-openapi.yml, openapi/availity-service-reviews-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/availity-claim-attachments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.availity.com/availity/v1/token\n- name: oauth2\n  source: openapi/availity-claim-status-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.availity.com/availity/v1/token\n- name: oauth2\n  source: openapi/availity-eligibility-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.availity.com/availity/v1/token\n- name: oauth2\n  source: openapi/availity-service-reviews-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.availity.com/availity/v1/token\nscopes:\n- scope: hipaa\n  description: Access to HIPAA transaction APIs\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/availity-claim-attachments-openapi.yml\n  - openapi/availity-claim-status-openapi.yml\n  - openapi/availity-eligibility-openapi.yml\n  - openapi/availity-service-reviews-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/scopes/availity-scopes.yml
summary_line: 1 scope · clientCredentials
tags: []
token_urls:
- https://api.availity.com/availity/v1/token
---
