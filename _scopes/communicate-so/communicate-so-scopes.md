---
api_specs:
- filename: communicate-so-account-credentials-api-openapi.yml
  format: yaml
  label: communicate-so Account credentials API
  slug: communicate-so-account-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-credentials-api-openapi.yml
- filename: communicate-so-account-preferences-api-openapi.yml
  format: yaml
  label: communicate-so Account preferences API
  slug: communicate-so-account-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-preferences-api-openapi.yml
- filename: communicate-so-agents-api-openapi.yml
  format: yaml
  label: communicate-so Agents API
  slug: communicate-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-agents-api-openapi.yml
- filename: communicate-so-authentication-api-openapi.yml
  format: yaml
  label: communicate-so Authentication API
  slug: communicate-so-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-authentication-api-openapi.yml
- filename: communicate-so-chat-api-openapi.yml
  format: yaml
  label: communicate-so Chat API
  slug: communicate-so-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-chat-api-openapi.yml
- filename: communicate-so-discovery-api-openapi.yml
  format: yaml
  label: communicate-so Discovery API
  slug: communicate-so-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-discovery-api-openapi.yml
- filename: communicate-so-grill-api-openapi.yml
  format: yaml
  label: communicate-so Grill API
  slug: communicate-so-grill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-grill-api-openapi.yml
- filename: communicate-so-inbox-api-openapi.yml
  format: yaml
  label: communicate-so Inbox API
  slug: communicate-so-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-inbox-api-openapi.yml
- filename: communicate-so-learnings-api-openapi.yml
  format: yaml
  label: communicate-so Learnings API
  slug: communicate-so-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-learnings-api-openapi.yml
- filename: communicate-so-notifications-api-openapi.yml
  format: yaml
  label: communicate-so Notifications API
  slug: communicate-so-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-notifications-api-openapi.yml
- filename: communicate-so-sources-api-openapi.yml
  format: yaml
  label: communicate-so Sources API
  slug: communicate-so-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-sources-api-openapi.yml
- filename: communicate-so-teams-api-openapi.yml
  format: yaml
  label: communicate-so Teams API
  slug: communicate-so-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-teams-api-openapi.yml
- filename: communicate-so-workspace-members-api-openapi.yml
  format: yaml
  label: communicate-so Workspace members API
  slug: communicate-so-workspace-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspace-members-api-openapi.yml
- filename: communicate-so-workspaces-api-openapi.yml
  format: yaml
  label: communicate-so Workspaces API
  slug: communicate-so-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspaces-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Communicate So Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'communicate-so publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the communicate-so API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: communicate-so
provider_slug: communicate-so
schemes: []
scope_count: 2
scope_names:
- agents:read
- chat:write
scopes:
- description: List agents in the workspace
  flows: []
  scope: agents:read
- description: Send chat turns to workspace agents
  flows: []
  scope: chat:write
slug: communicate-so-scopes
source_filename: communicate-so-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://developer.communicate.so/docs/authentication.md\nscopes:\n  - name: agents:read\n    description: List agents in the workspace\n  - name: chat:write\n    description: Send chat turns to workspace agents\n"
source_yaml_url: https://artifacts.apis.io/communicate-so/scopes/communicate-so-scopes.yml
summary_line: 2 scopes
tags:
- AI
- Customer Support
- Chatbot
- SaaS
- Automation
token_bound: false
token_urls: []
---
