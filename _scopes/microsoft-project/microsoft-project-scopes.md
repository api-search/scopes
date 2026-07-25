---
api_specs:
- filename: microsoft-project-assignments-api-openapi.yml
  format: yaml
  label: Microsoft Project Assignments API
  slug: microsoft-project-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-assignments-api-openapi.yml
- filename: microsoft-project-calendars-api-openapi.yml
  format: yaml
  label: Microsoft Project Calendars API
  slug: microsoft-project-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-calendars-api-openapi.yml
- filename: microsoft-project-custom-fields-api-openapi.yml
  format: yaml
  label: Microsoft Project Custom Fields API
  slug: microsoft-project-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-custom-fields-api-openapi.yml
- filename: microsoft-project-enterprise-project-types-api-openapi.yml
  format: yaml
  label: Microsoft Project Enterprise Project Types API
  slug: microsoft-project-enterprise-project-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-enterprise-project-types-api-openapi.yml
- filename: microsoft-project-event-handlers-api-openapi.yml
  format: yaml
  label: Microsoft Project Event Handlers API
  slug: microsoft-project-event-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-event-handlers-api-openapi.yml
- filename: microsoft-project-lookup-tables-api-openapi.yml
  format: yaml
  label: Microsoft Project Lookup Tables API
  slug: microsoft-project-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-lookup-tables-api-openapi.yml
- filename: microsoft-project-phases-api-openapi.yml
  format: yaml
  label: Microsoft Project Phases API
  slug: microsoft-project-phases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-phases-api-openapi.yml
- filename: microsoft-project-projects-api-openapi.yml
  format: yaml
  label: Microsoft Project Projects API
  slug: microsoft-project-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-projects-api-openapi.yml
- filename: microsoft-project-resources-api-openapi.yml
  format: yaml
  label: Microsoft Project Resources API
  slug: microsoft-project-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-resources-api-openapi.yml
- filename: microsoft-project-stages-api-openapi.yml
  format: yaml
  label: Microsoft Project Stages API
  slug: microsoft-project-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-stages-api-openapi.yml
- filename: microsoft-project-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Project Tasks API
  slug: microsoft-project-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-tasks-api-openapi.yml
- filename: microsoft-project-timesheets-api-openapi.yml
  format: yaml
  label: Microsoft Project Timesheets API
  slug: microsoft-project-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-timesheets-api-openapi.yml
- filename: microsoft-project-workflow-activities-api-openapi.yml
  format: yaml
  label: Microsoft Project Workflow Activities API
  slug: microsoft-project-workflow-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-workflow-activities-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Project Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Project publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Project API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Project
provider_slug: microsoft-project
schemes:
- description: OAuth 2.0 authentication via Azure AD for SharePoint Online
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: oauth2
  source: openapi/microsoft-project-rest-api.yaml
scope_count: 2
scope_names:
- ProjectServer.Read
- ProjectServer.ReadWrite
scopes:
- description: Read Project Server data
  flows:
  - authorizationCode
  scope: ProjectServer.Read
- description: Read and write Project Server data
  flows:
  - authorizationCode
  scope: ProjectServer.ReadWrite
slug: microsoft-project-scopes
source_filename: microsoft-project-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-project-rest-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-project-rest-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n  description: OAuth 2.0 authentication via Azure AD for SharePoint Online\nscopes:\n- scope: ProjectServer.Read\n  description: Read Project Server data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-project-rest-api.yaml\n- scope: ProjectServer.ReadWrite\n  description: Read and write Project Server data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-project-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/scopes/microsoft-project-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
token_urls:
- https://login.microsoftonline.com/common/oauth2/token
---
