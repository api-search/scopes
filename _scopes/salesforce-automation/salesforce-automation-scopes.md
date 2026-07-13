---
api_specs:
- filename: salesforce-rest-api-openapi.json
  format: json
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-rest-api-openapi.json
- filename: salesforce-bulk-api-openapi.json
  format: json
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-bulk-api-openapi.json
- filename: salesforce-streaming-api-openapi.json
  format: json
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-streaming-api-openapi.json
- filename: salesforce-platform-events-api-openapi.json
  format: json
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-platform-events-api-openapi.json
- filename: salesforce-analytics-api-openapi.json
  format: json
  label: Salesforce Analytics API
  slug: salesforce-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-analytics-api-openapi.json
- filename: salesforce-tooling-api-openapi.json
  format: json
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-tooling-api-openapi.json
- filename: salesforce-connect-rest-api-openapi.json
  format: json
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-connect-rest-api-openapi.json
- filename: salesforce-change-data-capture-api-openapi.json
  format: json
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-change-data-capture-api-openapi.json
- filename: salesforce-invocable-actions-api-openapi.json
  format: json
  label: Salesforce Invocable Actions API
  slug: salesforce-invocable-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-invocable-actions-api-openapi.json
- filename: salesforce-composite-api-openapi.json
  format: json
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-composite-api-openapi.json
- filename: salesforce-apex-rest-api-openapi.json
  format: json
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-apex-rest-api-openapi.json
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Automation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Automation publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Automation API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Automation
provider_slug: salesforce-automation
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-analytics-api-openapi.json
- description: Salesforce OAuth 2.0. The connected app must have API access enabled.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-apex-rest-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-bulk-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-change-data-capture-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-composite-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-connect-rest-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-invocable-actions-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-platform-events-api-openapi.json
- description: Salesforce OAuth 2.0 authentication. Supports Web Server Flow (authorization_code), User-Agent Flow (implicit), JWT Bearer Token Flow, and Device Flow.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-rest-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-streaming-api-openapi.json
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-tooling-api-openapi.json
scope_count: 5
scope_names:
- api
- chatter_api
- full
- refresh_token
- wave_api
scopes:
- description: Access and manage your Salesforce data
  flows:
  - authorizationCode
  scope: api
- description: Access Chatter REST API resources
  flows:
  - authorizationCode
  scope: chatter_api
- description: Full access to your Salesforce data
  flows:
  - authorizationCode
  scope: full
- description: Perform requests at any time on your behalf
  flows:
  - authorizationCode
  scope: refresh_token
- description: Access CRM Analytics REST API resources
  flows:
  - authorizationCode
  scope: wave_api
slug: salesforce-automation-scopes
source_filename: salesforce-automation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-analytics-api-openapi.json, openapi/salesforce-apex-rest-api-openapi.json,\n  openapi/salesforce-bulk-api-openapi.json, openapi/salesforce-change-data-capture-api-openapi.json,\n  openapi/salesforce-composite-api-openapi.json, openapi/salesforce-connect-rest-api-openapi.json,\n  openapi/salesforce-invocable-actions-api-openapi.json, openapi/salesforce-platform-events-api-openapi.json,\n  openapi/salesforce-rest-api-openapi.json, openapi/salesforce-streaming-api-openapi.json, openapi/salesforce-tooling-api-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/salesforce-analytics-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-apex-rest-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0. The connected app must have API access enabled.\n- name: oauth2\n  source: openapi/salesforce-bulk-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-change-data-capture-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-composite-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n\
  \  source: openapi/salesforce-connect-rest-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-invocable-actions-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-platform-events-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-rest-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n\
  \  description: Salesforce OAuth 2.0 authentication. Supports Web Server Flow (authorization_code),\n    User-Agent Flow (implicit), JWT Bearer Token Flow, and Device Flow.\n- name: oauth2\n  source: openapi/salesforce-streaming-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n- name: oauth2\n  source: openapi/salesforce-tooling-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Access and manage your Salesforce data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-analytics-api-openapi.json\n  - openapi/salesforce-apex-rest-api-openapi.json\n  - openapi/salesforce-bulk-api-openapi.json\n  - openapi/salesforce-change-data-capture-api-openapi.json\n\
  \  - openapi/salesforce-composite-api-openapi.json\n  - openapi/salesforce-connect-rest-api-openapi.json\n  - openapi/salesforce-invocable-actions-api-openapi.json\n  - openapi/salesforce-platform-events-api-openapi.json\n  - openapi/salesforce-rest-api-openapi.json\n  - openapi/salesforce-streaming-api-openapi.json\n  - openapi/salesforce-tooling-api-openapi.json\n- scope: chatter_api\n  description: Access Chatter REST API resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-connect-rest-api-openapi.json\n- scope: full\n  description: Full access to your Salesforce data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-rest-api-openapi.json\n- scope: refresh_token\n  description: Perform requests at any time on your behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-rest-api-openapi.json\n- scope: wave_api\n  description: Access CRM Analytics REST API resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-analytics-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/scopes/salesforce-automation-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Automation
- Cloud
- CRM
- Enterprise
- Sales
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
