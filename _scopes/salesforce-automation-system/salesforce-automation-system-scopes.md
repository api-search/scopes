---
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
name: Salesforce Automation System Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Automation System publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Automation System API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Automation System
provider_slug: salesforce-automation-system
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-automation-flow-openapi.yml
scope_count: 2
scope_names:
- api
- refresh_token
scopes:
- description: Access and manage your data
  flows:
  - authorizationCode
  - clientCredentials
  scope: api
- description: Perform requests at any time
  flows:
  - authorizationCode
  scope: refresh_token
slug: salesforce-automation-system-scopes
source_filename: salesforce-automation-system-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-automation-flow-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-automation-flow-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Access and manage your data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/salesforce-automation-flow-openapi.yml\n- scope: refresh_token\n  description: Perform requests at any time\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-automation-flow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation-system/refs/heads/main/scopes/salesforce-automation-system-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Approval Process
- Automation
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
