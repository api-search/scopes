---
api_specs:
- filename: kanera-app-activity-api-openapi.yml
  format: yaml
  label: Kanera Activity API
  slug: kanera-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-activity-api-openapi.yml
- filename: kanera-app-agent-runs-api-openapi.yml
  format: yaml
  label: Kanera Agent Runs API
  slug: kanera-app-agent-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-agent-runs-api-openapi.yml
- filename: kanera-app-attachments-api-openapi.yml
  format: yaml
  label: Kanera Attachments API
  slug: kanera-app-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-attachments-api-openapi.yml
- filename: kanera-app-authentication-api-openapi.yml
  format: yaml
  label: Kanera Authentication API
  slug: kanera-app-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-authentication-api-openapi.yml
- filename: kanera-app-automations-api-openapi.yml
  format: yaml
  label: Kanera Automations API
  slug: kanera-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-automations-api-openapi.yml
- filename: kanera-app-board-access-api-openapi.yml
  format: yaml
  label: Kanera Board Access API
  slug: kanera-app-board-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-board-access-api-openapi.yml
- filename: kanera-app-boards-api-openapi.yml
  format: yaml
  label: Kanera Boards API
  slug: kanera-app-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-boards-api-openapi.yml
- filename: kanera-app-card-labels-api-openapi.yml
  format: yaml
  label: Kanera Card Labels API
  slug: kanera-app-card-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-card-labels-api-openapi.yml
- filename: kanera-app-cards-api-openapi.yml
  format: yaml
  label: Kanera Cards API
  slug: kanera-app-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-cards-api-openapi.yml
- filename: kanera-app-comments-api-openapi.yml
  format: yaml
  label: Kanera Comments API
  slug: kanera-app-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-comments-api-openapi.yml
- filename: kanera-app-custom-fields-api-openapi.yml
  format: yaml
  label: Kanera Custom Fields API
  slug: kanera-app-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-custom-fields-api-openapi.yml
- filename: kanera-app-external-links-api-openapi.yml
  format: yaml
  label: Kanera External Links API
  slug: kanera-app-external-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-external-links-api-openapi.yml
- filename: kanera-app-following-api-openapi.yml
  format: yaml
  label: Kanera Following API
  slug: kanera-app-following-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-following-api-openapi.yml
- filename: kanera-app-health-api-openapi.yml
  format: yaml
  label: Kanera Health API
  slug: kanera-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-health-api-openapi.yml
- filename: kanera-app-lists-api-openapi.yml
  format: yaml
  label: Kanera Lists API
  slug: kanera-app-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-lists-api-openapi.yml
- filename: kanera-app-media-api-openapi.yml
  format: yaml
  label: Kanera Media API
  slug: kanera-app-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-media-api-openapi.yml
- filename: kanera-app-notes-api-openapi.yml
  format: yaml
  label: Kanera Notes API
  slug: kanera-app-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-notes-api-openapi.yml
- filename: kanera-app-scratchpad-api-openapi.yml
  format: yaml
  label: Kanera Scratchpad API
  slug: kanera-app-scratchpad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-scratchpad-api-openapi.yml
- filename: kanera-app-search-api-openapi.yml
  format: yaml
  label: Kanera Search API
  slug: kanera-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-search-api-openapi.yml
- filename: kanera-app-separators-api-openapi.yml
  format: yaml
  label: Kanera Separators API
  slug: kanera-app-separators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-separators-api-openapi.yml
- filename: kanera-app-webhooks-api-openapi.yml
  format: yaml
  label: Kanera Webhooks API
  slug: kanera-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-webhooks-api-openapi.yml
- filename: kanera-app-workspaces-api-openapi.yml
  format: yaml
  label: Kanera Workspaces API
  slug: kanera-app-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kanera-app/openapi/kanera-app-workspaces-api-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Kanera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kanera publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kanera API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kanera
provider_slug: kanera-app
schemes:
- description: Short-lived user or workspace-service OAuth tokens.
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: KaneraOAuth
  source: openapi/kanera-app-openapi.json
scope_count: 3
scope_names:
- kanera:admin
- kanera:read
- kanera:write
scopes:
- description: Perform supported workspace-admin API operations.
  flows:
  - clientCredentials
  scope: kanera:admin
- description: Read accessible Kanera project data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: kanera:read
- description: Create and update accessible Kanera content, including supported workspace administration where the authorizing user is an administrator.
  flows:
  - authorizationCode
  - clientCredentials
  scope: kanera:write
slug: kanera-app-scopes
source_filename: kanera-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kanera-app-openapi.json\nschemes:\n- name: KaneraOAuth\n  source: openapi/kanera-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: Short-lived user or workspace-service OAuth tokens.\nscopes:\n- scope: kanera:admin\n  description: Perform supported workspace-admin API operations.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kanera-app-openapi.json\n- scope: kanera:read\n  description: Read accessible Kanera project data.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/kanera-app-openapi.json\n- scope: kanera:write\n  description: Create and update accessible Kanera content, including supported workspace administration\n    where the authorizing user is an administrator.\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/kanera-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kanera-app/scopes/kanera-app-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Project Management
- Collaboration
- Artificial Intelligence
- Automation
token_bound: false
token_urls:
- /oauth/token
---
