---
api_specs:
- filename: salesforce-knowledge-management-rest-api-openapi.yml
  format: yaml
  label: Salesforce Knowledge REST API
  slug: salesforce-knowledge-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/openapi/salesforce-knowledge-management-rest-api-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Knowledge Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Knowledge Management publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Knowledge Management API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-knowledge-management-rest-api-openapi.yml
scope_count: 2
scope_names:
- api
- full
scopes:
- description: Access and manage your data
  flows:
  - authorizationCode
  scope: api
- description: Full access
  flows:
  - authorizationCode
  scope: full
slug: salesforce-knowledge-management-scopes
source_filename: salesforce-knowledge-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-knowledge-management-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-knowledge-management-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Access and manage your data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-knowledge-management-rest-api-openapi.yml\n- scope: full\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-knowledge-management-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/scopes/salesforce-knowledge-management-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
