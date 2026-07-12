---
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Net Zero Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Net Zero Cloud publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Net Zero Cloud API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Net Zero Cloud
provider_slug: salesforce-net-zero-cloud
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-net-zero-cloud-rest-api-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Access and manage your data
  flows:
  - authorizationCode
  scope: api
slug: salesforce-net-zero-cloud-scopes
source_filename: salesforce-net-zero-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Access and manage your data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-net-zero-cloud-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/scopes/salesforce-net-zero-cloud-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Environmental
- ESG
- Net Zero
- Sustainability
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
