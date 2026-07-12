---
authorization_urls:
- https://app.smartsheet.com/b/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Smartsheet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Smartsheet publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Smartsheet API on a user''s behalf.


  Tokens are issued from https://api.smartsheet.com/2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Smartsheet
provider_slug: smartsheet
schemes:
- description: Smartsheet OAuth 2.0 authorization.
  flows:
  - authorizationUrl: https://app.smartsheet.com/b/authorize
    flow: authorizationCode
    tokenUrl: https://api.smartsheet.com/2.0/token
  name: OAuth2
  source: openapi/smartsheet-openapi.yml
scope_count: 10
scope_names:
- ADMIN_SHEETS
- ADMIN_USERS
- ADMIN_WEBHOOKS
- ADMIN_WORKSPACES
- DELETE_SHEETS
- READ_CONTACTS
- READ_SHEETS
- READ_USERS
- SHARE_SHEETS
- WRITE_SHEETS
scopes:
- description: Sheet admin
  flows:
  - authorizationCode
  scope: ADMIN_SHEETS
- description: User admin
  flows:
  - authorizationCode
  scope: ADMIN_USERS
- description: Webhook admin
  flows:
  - authorizationCode
  scope: ADMIN_WEBHOOKS
- description: Workspace admin
  flows:
  - authorizationCode
  scope: ADMIN_WORKSPACES
- description: Delete sheets
  flows:
  - authorizationCode
  scope: DELETE_SHEETS
- description: View contacts
  flows:
  - authorizationCode
  scope: READ_CONTACTS
- description: View sheets
  flows:
  - authorizationCode
  scope: READ_SHEETS
- description: View users
  flows:
  - authorizationCode
  scope: READ_USERS
- description: Share sheets
  flows:
  - authorizationCode
  scope: SHARE_SHEETS
- description: Edit sheets
  flows:
  - authorizationCode
  scope: WRITE_SHEETS
slug: smartsheet-scopes
source_filename: smartsheet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartsheet-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/smartsheet-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.smartsheet.com/b/authorize\n    tokenUrl: https://api.smartsheet.com/2.0/token\n  description: Smartsheet OAuth 2.0 authorization.\nscopes:\n- scope: ADMIN_SHEETS\n  description: Sheet admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: ADMIN_USERS\n  description: User admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: ADMIN_WEBHOOKS\n  description: Webhook admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: ADMIN_WORKSPACES\n  description: Workspace admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: DELETE_SHEETS\n  description: Delete sheets\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: READ_CONTACTS\n  description: View contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: READ_SHEETS\n  description: View sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: READ_USERS\n  description: View users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: SHARE_SHEETS\n  description: Share sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n- scope: WRITE_SHEETS\n  description: Edit sheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartsheet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartsheet/refs/heads/main/scopes/smartsheet-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow Automation
- Spreadsheets
token_urls:
- https://api.smartsheet.com/2.0/token
---
