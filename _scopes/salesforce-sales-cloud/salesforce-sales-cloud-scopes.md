---
api_specs:
- filename: salesforce-sales-cloud-rest-api-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-rest-api-openapi.yml
- filename: salesforce-sales-cloud-bulk-api-openapi.yml
  format: yaml
  label: Bulk API 2.0
  slug: bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-bulk-api-openapi.yml
- filename: salesforce-sales-cloud-platform-events-api-openapi.yml
  format: yaml
  label: Platform Events API
  slug: platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
- filename: salesforce-sales-cloud-analytics-api-openapi.yml
  format: yaml
  label: Analytics REST API
  slug: analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-analytics-api-openapi.yml
- filename: salesforce-sales-cloud-composite-api-openapi.yml
  format: yaml
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-composite-api-openapi.yml
- filename: salesforce-sales-cloud-graphql-api-openapi.yml
  format: yaml
  label: Salesforce GraphQL API
  slug: salesforce-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-graphql-api-openapi.yml
- filename: salesforce-sales-cloud-tooling-api-openapi.yml
  format: yaml
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-tooling-api-openapi.yml
- filename: salesforce-sales-cloud-change-data-capture-api-openapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
- filename: salesforce-sales-cloud-connect-api-openapi.yml
  format: yaml
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-connect-api-openapi.yml
- filename: salesforce-sales-cloud-ui-api-openapi.yml
  format: yaml
  label: Salesforce User Interface API
  slug: salesforce-user-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-ui-api-openapi.yml
- filename: salesforce-sales-cloud-apex-rest-api-openapi.yml
  format: yaml
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Sales Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Sales Cloud publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Sales Cloud API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schemes:
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-analytics-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-bulk-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-composite-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-connect-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-graphql-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-rest-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-tooling-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-sales-cloud-ui-api-openapi.yml
scope_count: 4
scope_names:
- api
- chatter_api
- full
- refresh_token
scopes:
- description: Access and manage your Salesforce data
  flows:
  - authorizationCode
  - clientCredentials
  scope: api
- description: Access Chatter data
  flows:
  - authorizationCode
  scope: chatter_api
- description: Full access to your Salesforce data
  flows:
  - authorizationCode
  scope: full
- description: Allow refresh token access
  flows:
  - authorizationCode
  scope: refresh_token
slug: salesforce-sales-cloud-scopes
source_filename: salesforce-sales-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-sales-cloud-analytics-api-openapi.yml, openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml,\n  openapi/salesforce-sales-cloud-bulk-api-openapi.yml, openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml,\n  openapi/salesforce-sales-cloud-composite-api-openapi.yml, openapi/salesforce-sales-cloud-connect-api-openapi.yml,\n  openapi/salesforce-sales-cloud-graphql-api-openapi.yml, openapi/salesforce-sales-cloud-platform-events-api-openapi.yml,\n  openapi/salesforce-sales-cloud-rest-api-openapi.yml, openapi/salesforce-sales-cloud-tooling-api-openapi.yml,\n  openapi/salesforce-sales-cloud-ui-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-analytics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description:\
  \ Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-bulk-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n\
  - name: oauth2\n  source: openapi/salesforce-sales-cloud-composite-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-connect-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-graphql-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-platform-events-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-tooling-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-sales-cloud-ui-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\nscopes:\n- scope: api\n  description: Access and manage your Salesforce data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/salesforce-sales-cloud-analytics-api-openapi.yml\n  - openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml\n  - openapi/salesforce-sales-cloud-bulk-api-openapi.yml\n  - openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml\n  - openapi/salesforce-sales-cloud-composite-api-openapi.yml\n  - openapi/salesforce-sales-cloud-connect-api-openapi.yml\n  - openapi/salesforce-sales-cloud-graphql-api-openapi.yml\n  - openapi/salesforce-sales-cloud-platform-events-api-openapi.yml\n  - openapi/salesforce-sales-cloud-rest-api-openapi.yml\n  - openapi/salesforce-sales-cloud-tooling-api-openapi.yml\n\
  \  - openapi/salesforce-sales-cloud-ui-api-openapi.yml\n- scope: chatter_api\n  description: Access Chatter data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-sales-cloud-connect-api-openapi.yml\n- scope: full\n  description: Full access to your Salesforce data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-sales-cloud-rest-api-openapi.yml\n- scope: refresh_token\n  description: Allow refresh token access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-sales-cloud-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/scopes/salesforce-sales-cloud-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
