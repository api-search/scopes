---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Healthcare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Healthcare publishes 2 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Healthcare API on a user''s behalf.


  Tokens are issued from https://accounts.google.com/o/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Healthcare
provider_slug: google-cloud-healthcare
schemes:
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/openapi-v1.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/openapi-v1.yaml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/openapi-v1beta1.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/openapi-v1beta1.yaml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-healthcare
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Read, write and manage healthcare data
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/cloud-healthcare
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-healthcare-scopes
source_filename: google-cloud-healthcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-v1.yaml, openapi/openapi-v1beta1.yaml\nschemes:\n- name: Oauth2\n  source: openapi/openapi-v1.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/openapi-v1.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/openapi-v1beta1.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/openapi-v1beta1.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n\
  \  description: Oauth 2.0 authorizationCode authentication\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-healthcare\n  description: Read, write and manage healthcare data\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/openapi-v1.yaml\n  - openapi/openapi-v1beta1.yaml\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/openapi-v1.yaml\n  - openapi/openapi-v1beta1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-healthcare/refs/heads/main/scopes/google-cloud-healthcare-scopes.yml
summary_line: 2 scopes · implicit/authorizationCode
tags:
- Healthcare
- FHIR
- HL7v2
- DICOM
- Medical Imaging
- De-identification
- Interoperability
- Cloud
token_urls:
- https://accounts.google.com/o/oauth2/token
---
