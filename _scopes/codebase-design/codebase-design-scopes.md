---
api_specs:
- filename: codebase-design-account-api-openapi.yml
  format: yaml
  label: Codebase Account API
  slug: codebase-design-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-account-api-openapi.yml
- filename: codebase-design-admin-api-openapi.yml
  format: yaml
  label: Codebase Admin API
  slug: codebase-design-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-admin-api-openapi.yml
- filename: codebase-design-api-keys-api-openapi.yml
  format: yaml
  label: Codebase API Keys API
  slug: codebase-design-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-api-keys-api-openapi.yml
- filename: codebase-design-billing-api-openapi.yml
  format: yaml
  label: Codebase Billing API
  slug: codebase-design-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-billing-api-openapi.yml
- filename: codebase-design-builds-api-openapi.yml
  format: yaml
  label: Codebase Builds API
  slug: codebase-design-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-builds-api-openapi.yml
- filename: codebase-design-community-api-openapi.yml
  format: yaml
  label: Codebase Community API
  slug: codebase-design-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-community-api-openapi.yml
- filename: codebase-design-credits-api-openapi.yml
  format: yaml
  label: Codebase Credits API
  slug: codebase-design-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-credits-api-openapi.yml
- filename: codebase-design-deploys-api-openapi.yml
  format: yaml
  label: Codebase Deploys API
  slug: codebase-design-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-deploys-api-openapi.yml
- filename: codebase-design-gallery-api-openapi.yml
  format: yaml
  label: Codebase Gallery API
  slug: codebase-design-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-gallery-api-openapi.yml
- filename: codebase-design-health-api-openapi.yml
  format: yaml
  label: Codebase Health API
  slug: codebase-design-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-health-api-openapi.yml
- filename: codebase-design-inference-api-openapi.yml
  format: yaml
  label: Codebase Inference API
  slug: codebase-design-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-inference-api-openapi.yml
- filename: codebase-design-platform-api-openapi.yml
  format: yaml
  label: Codebase Platform API
  slug: codebase-design-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-platform-api-openapi.yml
- filename: codebase-design-projects-api-openapi.yml
  format: yaml
  label: Codebase Projects API
  slug: codebase-design-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-projects-api-openapi.yml
- filename: codebase-design-prompts-api-openapi.yml
  format: yaml
  label: Codebase Prompts API
  slug: codebase-design-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-prompts-api-openapi.yml
- filename: codebase-design-sessions-api-openapi.yml
  format: yaml
  label: Codebase Sessions API
  slug: codebase-design-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-sessions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://codebase.design/agents
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Codebase Scopes
name_suffix: OAuth Scopes
note: The spec declares no oauth2 securityScheme; scopes are API-key scopes (also granted to OAuth tokens). Names come from the api-keys request schema enum in openapi/_original/codebase-design-openapi.json; descriptions only where /agents or the spec states them. The enum also lists an admin:* value.
overview: 'Codebase publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Codebase API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Codebase
provider_slug: codebase-design
schemes: []
scope_count: 14
scope_names:
- inference
- projects:read
- projects:write
- builds:read
- builds:write
- deploys:read
- deploys:write
- gallery:read
- gallery:write
- billing:read
- billing:write
- chat:read
- chat:write
- chat:admin
scopes:
- description: ''
  flows: []
  scope: inference
- description: Read projects; export source zip
  flows: []
  scope: projects:read
- description: Create/modify projects and files
  flows: []
  scope: projects:write
- description: Poll build status, stream events, open previews
  flows: []
  scope: builds:read
- description: Start, follow up, cancel, retry builds
  flows: []
  scope: builds:write
- description: Read deploy status and history
  flows: []
  scope: deploys:read
- description: Publish, roll back, take down sites; make a project public/unlisted. Not granted by default
  flows: []
  scope: deploys:write
- description: ''
  flows: []
  scope: gallery:read
- description: ''
  flows: []
  scope: gallery:write
- description: ''
  flows: []
  scope: billing:read
- description: Billing portal and checkout sessions
  flows: []
  scope: billing:write
- description: ''
  flows: []
  scope: chat:read
- description: ''
  flows: []
  scope: chat:write
- description: ''
  flows: []
  scope: chat:admin
slug: codebase-design-scopes
source_filename: codebase-design-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codebase.design/agents\ndocs: https://codebase.design/agents\nnote: The spec declares no oauth2 securityScheme; scopes are API-key scopes (also granted to OAuth tokens). Names\n  come from the api-keys request schema enum in openapi/_original/codebase-design-openapi.json; descriptions only\n  where /agents or the spec states them. The enum also lists an admin:* value.\nrecommended_agent_scopes:\n- builds:write\n- builds:read\n- projects:read\nscopes:\n- name: inference\n- name: projects:read\n  description: Read projects; export source zip\n- name: projects:write\n  description: Create/modify projects and files\n- name: builds:read\n  description: Poll build status, stream events, open previews\n- name: builds:write\n  description: Start, follow up, cancel, retry builds\n- name: deploys:read\n  description: Read deploy status and history\n- name: deploys:write\n  description: Publish, roll back, take down sites; make\
  \ a project public/unlisted. Not granted by default\n- name: gallery:read\n- name: gallery:write\n- name: billing:read\n- name: billing:write\n  description: Billing portal and checkout sessions\n- name: chat:read\n- name: chat:write\n- name: chat:admin\n"
source_yaml_url: https://artifacts.apis.io/codebase-design/scopes/codebase-design-scopes.yml
summary_line: 14 scopes
tags:
- Company
- AI App Builder
- Code Generation
- Developer Tools
- Open-Weight Models
- CLI
- MCP
- Web3
token_bound: false
token_urls: []
---
