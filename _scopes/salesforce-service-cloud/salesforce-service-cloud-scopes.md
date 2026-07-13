---
api_specs:
- filename: resources_list.htm
  format: yaml
  label: Salesforce Service Cloud REST API
  slug: salesforce-service-cloud-rest-api
  spec_type: OpenAPI
  url: https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/resources_list.htm
- filename: salesforce-streaming-api-asyncapi.yml
  format: yaml
  label: Service Cloud Streaming API
  slug: service-cloud-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/asyncapi/salesforce-streaming-api-asyncapi.yml
- filename: salesforce-live-agent-openapi.yml
  format: yaml
  label: Live Agent REST API
  slug: live-agent-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-live-agent-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Service Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Service Cloud publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Service Cloud API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Service Cloud
provider_slug: salesforce-service-cloud
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-service-cloud-rest-openapi.yml
scope_count: 2
scope_names:
- api
- full
scopes:
- description: Access Salesforce REST API
  flows:
  - authorizationCode
  scope: api
- description: Full access
  flows:
  - authorizationCode
  scope: full
slug: salesforce-service-cloud-scopes
source_filename: salesforce-service-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-service-cloud-rest-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-service-cloud-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Access Salesforce REST API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-service-cloud-rest-openapi.yml\n- scope: full\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-service-cloud-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/scopes/salesforce-service-cloud-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Case Management
- CRM
- Customer Service
- Help Desk
- Support
- Ticketing
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
