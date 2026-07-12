---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Logging Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Logging publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Logging API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-cloud-logging-openapi.yml
scope_count: 4
scope_names:
- cloud-platform
- logging.admin
- logging.read
- logging.write
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: cloud-platform
- description: Administrate logs
  flows:
  - authorizationCode
  scope: logging.admin
- description: View logs
  flows:
  - authorizationCode
  scope: logging.read
- description: Submit log data
  flows:
  - authorizationCode
  scope: logging.write
slug: google-cloud-logging-scopes
source_filename: google-cloud-logging-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-logging-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-cloud-logging-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-logging-openapi.yml\n- scope: logging.admin\n  description: Administrate logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-logging-openapi.yml\n- scope: logging.read\n  description: View logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-logging-openapi.yml\n- scope: logging.write\n  description: Submit log data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-logging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/scopes/google-cloud-logging-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Cloud
- Logging
- Monitoring
- Observability
token_urls:
- https://oauth2.googleapis.com/token
---
