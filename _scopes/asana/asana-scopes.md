---
authorization_urls:
- https://app.asana.com/-/oauth_authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Asana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Asana publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Asana API on a user''s behalf.


  Tokens are issued from https://app.asana.com/-/oauth_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Asana
provider_slug: asana
schemes:
- description: OAuth 2.0 authorization code flow.
  flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-allocations-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-attachments-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-batch-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-custom-fields-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-enum-options-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-events-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-goal-relationships-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-goals-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-jobs-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-memberships-api-openapi.yml
- description: 'We require that applications designed to access the Asana API on behalf of multiple users implement OAuth 2.0.

    Asana supports the Authorization Code Grant flow.'
  flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-organization-exports-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-portfolios-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-project-templates-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-rule-triggers-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-sections-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-status-updates-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-tags-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-task-templates-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-tasks-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-teams-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-time-periods-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-time-tracking-entries-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-user-task-lists-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-users-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-webhooks-api-openapi.yml
- flows:
  - authorizationUrl: https://app.asana.com/-/oauth_authorize
    flow: authorizationCode
    tokenUrl: https://app.asana.com/-/oauth_token
  name: oauth2
  source: openapi/asana-workspaces-api-openapi.yml
scope_count: 18
scope_names:
- attachments:write
- default
- email
- goals:read
- openid
- portfolios:read
- profile
- project_templates:read
- projects:delete
- projects:read
- projects:write
- stories:read
- tasks:delete
- tasks:read
- tasks:write
- teams:read
- users:read
- workspaces:read
scopes:
- description: Create and modify access to attachments
  flows:
  - authorizationCode
  scope: attachments:write
- description: Provides access to all endpoints documented in the API reference.
  flows:
  - authorizationCode
  scope: default
- description: Provides access to the user’s email through the OpenID Connect user info endpoint.
  flows:
  - authorizationCode
  scope: email
- description: View access to goals
  flows:
  - authorizationCode
  scope: goals:read
- description: Provides access to OpenID Connect ID tokens and the OpenID Connect user info endpoint.
  flows:
  - authorizationCode
  scope: openid
- description: View access to portfolios
  flows:
  - authorizationCode
  scope: portfolios:read
- description: Provides access to the user’s name and profile photo through the OpenID Connect user info endpoint.
  flows:
  - authorizationCode
  scope: profile
- description: View access to project templates
  flows:
  - authorizationCode
  scope: project_templates:read
- description: Delete access to projects
  flows:
  - authorizationCode
  scope: projects:delete
- description: View access to projects
  flows:
  - authorizationCode
  scope: projects:read
- description: Create and modify access to projects
  flows:
  - authorizationCode
  scope: projects:write
- description: View access to stories
  flows:
  - authorizationCode
  scope: stories:read
- description: Delete access to tasks
  flows:
  - authorizationCode
  scope: tasks:delete
- description: View access to tasks
  flows:
  - authorizationCode
  scope: tasks:read
- description: Create and modify access to tasks
  flows:
  - authorizationCode
  scope: tasks:write
- description: View access to teams
  flows:
  - authorizationCode
  scope: teams:read
- description: View access to users
  flows:
  - authorizationCode
  scope: users:read
- description: View access to workspaces
  flows:
  - authorizationCode
  scope: workspaces:read
slug: asana-scopes
source_filename: asana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/asana-allocations-api-openapi.yml, openapi/asana-attachments-api-openapi.yml,\n  openapi/asana-batch-api-openapi.yml, openapi/asana-custom-fields-api-openapi.yml, openapi/asana-enum-options-api-openapi.yml,\n  openapi/asana-events-api-openapi.yml, openapi/asana-goal-relationships-api-openapi.yml, openapi/asana-goals-api-openapi.yml,\n  openapi/asana-jobs-api-openapi.yml, openapi/asana-memberships-api-openapi.yml, openapi/asana-openapi.yml,\n  openapi/asana-organization-exports-api-openapi.yml, openapi/asana-portfolios-api-openapi.yml,\n  openapi/asana-project-templates-api-openapi.yml, openapi/asana-projects-api-openapi.yml, openapi/asana-rule-triggers-api-openapi.yml,\n  openapi/asana-sections-api-openapi.yml, openapi/asana-status-updates-api-openapi.yml, openapi/asana-tags-api-openapi.yml,\n  openapi/asana-task-templates-api-openapi.yml, openapi/asana-tasks-api-openapi.yml, openapi/asana-teams-api-openapi.yml,\n  openapi/asana-time-periods-api-openapi.yml,\
  \ openapi/asana-time-tracking-entries-api-openapi.yml,\n  openapi/asana-user-task-lists-api-openapi.yml, openapi/asana-users-api-openapi.yml, openapi/asana-webhooks-api-openapi.yml,\n  openapi/asana-workspaces-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/asana-allocations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n  description: OAuth 2.0 authorization code flow.\n- name: oauth2\n  source: openapi/asana-attachments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-batch-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-custom-fields-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-enum-options-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-goal-relationships-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-goals-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl:\
  \ https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-jobs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-memberships-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n  description: |-\n    We require that applications designed to access the Asana API on behalf of multiple users implement OAuth 2.0.\n    Asana supports the Authorization Code Grant flow.\n- name: oauth2\n  source: openapi/asana-organization-exports-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-portfolios-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-project-templates-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-rule-triggers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n\
  \  source: openapi/asana-sections-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-status-updates-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-tags-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-task-templates-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-tasks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n\
  \    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-teams-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-time-periods-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-time-tracking-entries-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-user-task-lists-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-users-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-webhooks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\n- name: oauth2\n  source: openapi/asana-workspaces-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.asana.com/-/oauth_authorize\n    tokenUrl: https://app.asana.com/-/oauth_token\nscopes:\n- scope: attachments:write\n  description: Create and modify access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: default\n  description: Provides access to all endpoints documented in the API reference.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-allocations-api-openapi.yml\n  - openapi/asana-attachments-api-openapi.yml\n\
  \  - openapi/asana-batch-api-openapi.yml\n  - openapi/asana-custom-fields-api-openapi.yml\n  - openapi/asana-enum-options-api-openapi.yml\n  - openapi/asana-events-api-openapi.yml\n  - openapi/asana-goal-relationships-api-openapi.yml\n  - openapi/asana-goals-api-openapi.yml\n  - openapi/asana-jobs-api-openapi.yml\n  - openapi/asana-memberships-api-openapi.yml\n  - openapi/asana-openapi.yml\n  - openapi/asana-organization-exports-api-openapi.yml\n  - openapi/asana-portfolios-api-openapi.yml\n  - openapi/asana-project-templates-api-openapi.yml\n  - openapi/asana-projects-api-openapi.yml\n  - openapi/asana-rule-triggers-api-openapi.yml\n  - openapi/asana-sections-api-openapi.yml\n  - openapi/asana-status-updates-api-openapi.yml\n  - openapi/asana-tags-api-openapi.yml\n  - openapi/asana-task-templates-api-openapi.yml\n  - openapi/asana-tasks-api-openapi.yml\n  - openapi/asana-teams-api-openapi.yml\n  - openapi/asana-time-periods-api-openapi.yml\n  - openapi/asana-time-tracking-entries-api-openapi.yml\n\
  \  - openapi/asana-user-task-lists-api-openapi.yml\n  - openapi/asana-users-api-openapi.yml\n  - openapi/asana-webhooks-api-openapi.yml\n  - openapi/asana-workspaces-api-openapi.yml\n- scope: email\n  description: Provides access to the user’s email through the OpenID Connect user info endpoint.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: goals:read\n  description: View access to goals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: openid\n  description: Provides access to OpenID Connect ID tokens and the OpenID Connect user info\n    endpoint.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: portfolios:read\n  description: View access to portfolios\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: profile\n  description: Provides access to the user’s name and profile photo through the OpenID Connect\n    user info endpoint.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: project_templates:read\n  description: View access to project templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: projects:delete\n  description: Delete access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: projects:read\n  description: View access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: projects:write\n  description: Create and modify access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: stories:read\n  description: View access to stories\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: tasks:delete\n  description: Delete access to tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: tasks:read\n  description: View access to tasks\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: tasks:write\n  description: Create and modify access to tasks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: teams:read\n  description: View access to teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: users:read\n  description: View access to users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n- scope: workspaces:read\n  description: View access to workspaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/asana-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/scopes/asana-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
token_urls:
- https://app.asana.com/-/oauth_token
---
