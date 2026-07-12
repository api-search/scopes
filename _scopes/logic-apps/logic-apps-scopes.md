---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Logic Apps Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Logic Apps publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Logic Apps API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Logic Apps
provider_slug: logic-apps
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: azureAD
  source: openapi/logic-apps-management-api-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Access Azure Service Management API
  flows:
  - authorizationCode
  scope: user_impersonation
slug: logic-apps-scopes
source_filename: logic-apps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logic-apps-management-api-openapi.yml\nschemes:\n- name: azureAD\n  source: openapi/logic-apps-management-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\nscopes:\n- scope: user_impersonation\n  description: Access Azure Service Management API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/logic-apps-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logic-apps/refs/heads/main/scopes/logic-apps-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Azure
- Enterprise
- iPaaS
- Integration
- Microsoft
- Workflow Automation
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
