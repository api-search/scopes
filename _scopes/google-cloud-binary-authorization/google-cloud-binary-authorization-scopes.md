---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Binary Authorization Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Binary Authorization publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Binary Authorization API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Binary Authorization
provider_slug: google-cloud-binary-authorization
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/binary-authorization-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Full access to Google Cloud
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-binary-authorization-scopes
source_filename: google-cloud-binary-authorization-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/binary-authorization-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/binary-authorization-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/binary-authorization-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-binary-authorization/refs/heads/main/scopes/google-cloud-binary-authorization-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Attestation
- Container Security
- DevSecOps
- Kubernetes
- Policy Enforcement
- Supply Chain Security
token_urls:
- https://oauth2.googleapis.com/token
---
