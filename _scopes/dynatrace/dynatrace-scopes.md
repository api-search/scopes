---
api_specs:
- filename: dynatrace-metrics-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Metrics API v2
  slug: dynatrace-metrics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-metrics-api-v2-openapi.yml
- filename: dynatrace-log-monitoring-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Log Monitoring API v2
  slug: dynatrace-log-monitoring-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-log-monitoring-api-v2-openapi.yml
- filename: dynatrace-account-management-api-openapi.yml
  format: yaml
  label: Dynatrace Account Management API
  slug: dynatrace-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-account-management-api-openapi.yml
- filename: dynatrace-events-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Events API v2
  slug: dynatrace-events-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-events-api-v2-openapi.yml
- filename: dynatrace-problems-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Problems API v2
  slug: dynatrace-problems-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-problems-api-v2-openapi.yml
- filename: dynatrace-entities-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Entities API v2
  slug: dynatrace-entities-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-entities-api-v2-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Dynatrace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dynatrace publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dynatrace API on a user''s behalf.


  Tokens are issued from https://sso.dynatrace.com/sso/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dynatrace
provider_slug: dynatrace
schemes:
- description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET operations, account-idm-write for POST/PUT/DELETE operations.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token
  name: oauth2
  source: openapi/dynatrace-account-management-api-openapi.yml
scope_count: 3
scope_names:
- account-env-read
- account-idm-read
- account-idm-write
scopes:
- description: Read access to environment information
  flows:
  - clientCredentials
  scope: account-env-read
- description: Read access to account identity and management data
  flows:
  - clientCredentials
  scope: account-idm-read
- description: Write access to manage users, groups, and permissions
  flows:
  - clientCredentials
  scope: account-idm-write
slug: dynatrace-scopes
source_filename: dynatrace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dynatrace-account-management-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/dynatrace-account-management-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token\n  description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials\n    flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET\n    operations, account-idm-write for POST/PUT/DELETE operations.'\nscopes:\n- scope: account-env-read\n  description: Read access to environment information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynatrace-account-management-api-openapi.yml\n- scope: account-idm-read\n  description: Read access to account identity and management data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynatrace-account-management-api-openapi.yml\n- scope: account-idm-write\n  description:\
  \ Write access to manage users, groups, and permissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dynatrace-account-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/scopes/dynatrace-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
token_urls:
- https://sso.dynatrace.com/sso/oauth2/token
---
