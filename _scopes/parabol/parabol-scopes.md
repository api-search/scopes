---
api_specs:
- filename: parabol-graphql-subscriptions-asyncapi.yml
  format: yaml
  label: Parabol GraphQL API
  slug: parabol-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/asyncapi/parabol-graphql-subscriptions-asyncapi.yml
authorization_urls: []
description: ''
docs: https://raw.githubusercontent.com/ParabolInc/parabol/master/llms.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Parabol Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Parabol publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Parabol API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parabol
provider_slug: parabol
schemes:
- directive: '@scope(name: OAuthScopeEnum!)'
  name: PersonalAccessToken
  source: graphql/parabol-schema.graphql
  type: pat-scoped
scope_count: 16
scope_names:
- users:read
- users:write
- teams:read
- teams:write
- orgs:read
- orgs:write
- meetings:read
- meetings:write
- tasks:read
- tasks:write
- templates:read
- templates:write
- pages:read
- pages:write
- comments:read
- comments:write
scopes:
- description: Read user data
  flows: []
  scope: users:read
- description: Update user data
  flows: []
  scope: users:write
- description: Read team data
  flows: []
  scope: teams:read
- description: Create and update teams
  flows: []
  scope: teams:write
- description: Read organization data
  flows: []
  scope: orgs:read
- description: Update organization data
  flows: []
  scope: orgs:write
- description: Read meeting data
  flows: []
  scope: meetings:read
- description: Create and update meetings
  flows: []
  scope: meetings:write
- description: Read task data
  flows: []
  scope: tasks:read
- description: Create and update tasks
  flows: []
  scope: tasks:write
- description: Read meeting template data
  flows: []
  scope: templates:read
- description: Create and update meeting templates
  flows: []
  scope: templates:write
- description: Read page (document) data
  flows: []
  scope: pages:read
- description: Create and update pages
  flows: []
  scope: pages:write
- description: Read comment data
  flows: []
  scope: comments:read
- description: Create and update comments
  flows: []
  scope: comments:write
slug: parabol-scopes
source_filename: parabol-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: graphql/parabol-schema.graphql\ndocs: https://raw.githubusercontent.com/ParabolInc/parabol/master/llms.txt\nmodel: >-\n  Parabol Personal Access Tokens are scoped. Scopes are enforced in the GraphQL\n  schema via a `@scope(name: OAuthScopeEnum!)` directive on protected fields and\n  mutations. The enum below is the complete OAuthScopeEnum from the public\n  schema SDL; descriptions are from the published llms.txt scope table. These\n  are PAT scopes (not OAuth2 flow scopes) — Parabol has no OAuth2 flows yet.\nschemes:\n- name: PersonalAccessToken\n  type: pat-scoped\n  source: graphql/parabol-schema.graphql\n  directive: '@scope(name: OAuthScopeEnum!)'\nscopes:\n- scope: users:read\n  enum: USERS_READ\n  description: Read user data\n- scope: users:write\n  enum: USERS_WRITE\n  description: Update user data\n- scope: teams:read\n  enum: TEAMS_READ\n  description: Read team data\n- scope: teams:write\n  enum: TEAMS_WRITE\n  description:\
  \ Create and update teams\n- scope: orgs:read\n  enum: ORGS_READ\n  description: Read organization data\n- scope: orgs:write\n  enum: ORGS_WRITE\n  description: Update organization data\n- scope: meetings:read\n  enum: MEETINGS_READ\n  description: Read meeting data\n- scope: meetings:write\n  enum: MEETINGS_WRITE\n  description: Create and update meetings\n- scope: tasks:read\n  enum: TASKS_READ\n  description: Read task data\n- scope: tasks:write\n  enum: TASKS_WRITE\n  description: Create and update tasks\n- scope: templates:read\n  enum: TEMPLATES_READ\n  description: Read meeting template data\n- scope: templates:write\n  enum: TEMPLATES_WRITE\n  description: Create and update meeting templates\n- scope: pages:read\n  enum: PAGES_READ\n  description: Read page (document) data\n- scope: pages:write\n  enum: PAGES_WRITE\n  description: Create and update pages\n- scope: comments:read\n  enum: COMMENTS_READ\n  description: Read comment data\n- scope: comments:write\n  enum: COMMENTS_WRITE\n\
  \  description: Create and update comments\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/scopes/parabol-scopes.yml
summary_line: 16 scopes
tags:
- Company
- Developer Tools
- Agile
- Retrospectives
- Meetings
- Collaboration
- GraphQL
- Team Productivity
- Open Source
token_urls: []
---
