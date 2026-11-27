---
api_specs:
- filename: flowral-app-auth-api-openapi.yml
  format: yaml
  label: Flowral Auth API
  slug: flowral-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-auth-api-openapi.yml
- filename: flowral-app-brainstorms-api-openapi.yml
  format: yaml
  label: Flowral Brainstorms API
  slug: flowral-app-brainstorms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-brainstorms-api-openapi.yml
- filename: flowral-app-flows-api-openapi.yml
  format: yaml
  label: Flowral Flows API
  slug: flowral-app-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-flows-api-openapi.yml
- filename: flowral-app-notifications-api-openapi.yml
  format: yaml
  label: Flowral Notifications API
  slug: flowral-app-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-notifications-api-openapi.yml
- filename: flowral-app-search-api-openapi.yml
  format: yaml
  label: Flowral Search API
  slug: flowral-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-search-api-openapi.yml
- filename: flowral-app-tasks-api-openapi.yml
  format: yaml
  label: Flowral Tasks API
  slug: flowral-app-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-tasks-api-openapi.yml
- filename: flowral-app-team-api-openapi.yml
  format: yaml
  label: Flowral Team API
  slug: flowral-app-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-team-api-openapi.yml
- filename: flowral-app-templates-api-openapi.yml
  format: yaml
  label: Flowral Templates API
  slug: flowral-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-templates-api-openapi.yml
- filename: flowral-app-work-api-openapi.yml
  format: yaml
  label: Flowral Work API
  slug: flowral-app-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-work-api-openapi.yml
- filename: flowral-app-workspace-api-openapi.yml
  format: yaml
  label: Flowral Workspace API
  slug: flowral-app-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-workspace-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Flowral Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flowral publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flowral API on a user''s behalf.


  Tokens are issued from https://api.flowral.app/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flowral
provider_slug: flowral-app
schemes:
- description: Client credentials, for anything long-lived.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.flowral.app/v1/oauth/token
  name: oauth2
  source: openapi/flowral-app-openapi.json
scope_count: 8
scope_names:
- flows:read
- flows:write
- notifications:read
- notifications:write
- team:read
- team:write
- templates:read
- work:write
scopes:
- description: Read flows, tasks, schedules and reports
  flows:
  - clientCredentials
  scope: flows:read
- description: Create and change flows and tasks
  flows:
  - clientCredentials
  scope: flows:write
- description: Read what people are emailed about
  flows:
  - clientCredentials
  scope: notifications:read
- description: Change what people are emailed about
  flows:
  - clientCredentials
  scope: notifications:write
- description: Read members and invitations
  flows:
  - clientCredentials
  scope: team:read
- description: Invite people and change roles
  flows:
  - clientCredentials
  scope: team:write
- description: Read templates and start flows from them
  flows:
  - clientCredentials
  scope: templates:read
- description: Start, complete, assign and comment on work
  flows:
  - clientCredentials
  scope: work:write
slug: flowral-app-scopes
source_filename: flowral-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flowral-app-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/flowral-app-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flowral.app/v1/oauth/token\n  description: Client credentials, for anything long-lived.\nscopes:\n- scope: flows:read\n  description: Read flows, tasks, schedules and reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: flows:write\n  description: Create and change flows and tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: notifications:read\n  description: Read what people are emailed about\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: notifications:write\n  description: Change what people are emailed about\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: team:read\n  description:\
  \ Read members and invitations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: team:write\n  description: Invite people and change roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: templates:read\n  description: Read templates and start flows from them\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n- scope: work:write\n  description: Start, complete, assign and comment on work\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/flowral-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flowral-app/scopes/flowral-app-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- Project Management
- Software-as-a-Service
- Collaboration
- Agencies
- Team
token_bound: false
token_urls:
- https://api.flowral.app/v1/oauth/token
---
