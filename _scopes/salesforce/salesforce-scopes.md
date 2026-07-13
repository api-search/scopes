---
api_specs:
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
- filename: salesforce-bulk-api-2-openapi.yml
  format: yaml
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-bulk-api-2-openapi.yml
- filename: salesforce-streaming-asyncapi.yml
  format: yaml
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-streaming-asyncapi.yml
- filename: salesforce-platform-events-asyncapi.yml
  format: yaml
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-platform-events-asyncapi.yml
- filename: salesforce-change-data-capture-asyncapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-change-data-capture-asyncapi.yml
- filename: salesforce-ui-api-openapi.yml
  format: yaml
  label: Salesforce UI API
  slug: salesforce-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-ui-api-openapi.yml
- filename: salesforce-marketing-cloud-rest-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud REST API
  slug: salesforce-marketing-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-marketing-cloud-rest-openapi.yml
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce
  slug: salesforce-salesforce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
authorization_urls:
- '{DefaultParameterValue}{DefaultParameterValue}/services/oauth2/authorize'
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce
provider_slug: salesforce
schemes:
- flows:
  - authorizationUrl: '{DefaultParameterValue}{DefaultParameterValue}/services/oauth2/authorize'
    flow: implicit
  name: oauth2
  source: openapi/salesforce-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: ''
  flows:
  - implicit
  scope: api
slug: salesforce-scopes
source_filename: salesforce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: '{DefaultParameterValue}{DefaultParameterValue}/services/oauth2/authorize'\nscopes:\n- scope: api\n  flows:\n  - implicit\n  sources:\n  - openapi/salesforce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/scopes/salesforce-scopes.yml
summary_line: 1 scope · implicit
tags:
- Fortune 500
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
token_urls: []
---
