---
api_specs:
- filename: v12-documents-api-openapi.yml
  format: yaml
  label: V12 Documents API
  slug: v12-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-documents-api-openapi.yml
- filename: v12-findings-api-openapi.yml
  format: yaml
  label: V12 Findings API
  slug: v12-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-findings-api-openapi.yml
- filename: v12-me-api-openapi.yml
  format: yaml
  label: V12 Me API
  slug: v12-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-me-api-openapi.yml
- filename: v12-members-api-openapi.yml
  format: yaml
  label: V12 Members API
  slug: v12-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-members-api-openapi.yml
- filename: v12-repositories-api-openapi.yml
  format: yaml
  label: V12 Repositories API
  slug: v12-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-repositories-api-openapi.yml
- filename: v12-runs-api-openapi.yml
  format: yaml
  label: V12 Runs API
  slug: v12-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-runs-api-openapi.yml
- filename: v12-steers-api-openapi.yml
  format: yaml
  label: V12 Steers API
  slug: v12-steers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/openapi/v12-steers-api-openapi.yml
authorization_urls:
- https://v12.sh/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: V12 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'V12 publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the V12 API on a user''s behalf.


  Tokens are issued from https://v12.sh/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: V12
provider_slug: v12
schemes:
- flows:
  - authorizationUrl: https://v12.sh/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://v12.sh/api/oauth/token
  name: oauth2
  source: openapi/v12-openapi.json
scope_count: 10
scope_names:
- findings:read
- findings:write
- repos:read
- repos:write
- runs:manage
- runs:read
- runs:share
- runs:write
- steers:write
- user:read
scopes:
- description: 'The inbox: findings, their status, reports and comments.'
  flows:
  - authorizationCode
  scope: findings:read
- description: Change status, comment and update triage decisions.
  flows:
  - authorizationCode
  scope: findings:write
- description: Repositories, branches, pull requests, tags and Steer instructions.
  flows:
  - authorizationCode
  scope: repos:read
- description: Add public repositories to the workspace; owners can also add private repositories granted by GitHub, create repositories V12 hosts and push code to them.
  flows:
  - authorizationCode
  scope: repos:write
- description: Cancel runs.
  flows:
  - authorizationCode
  scope: runs:manage
- description: Runs, their progress and context documents.
  flows:
  - authorizationCode
  scope: runs:read
- description: Create, change and revoke guest links that open a run to people outside the organization.
  flows:
  - authorizationCode
  scope: runs:share
- description: Estimate and start runs; add or archive context documents.
  flows:
  - authorizationCode
  scope: runs:write
- description: Create, edit, archive and restore Steers. Archiving detaches them from Autopilot rules; finding tags and run history are kept.
  flows:
  - authorizationCode
  scope: steers:write
- description: 'The member directory: usernames, emails and roles. Any key reads its own account, organization and credit balance without it.'
  flows:
  - authorizationCode
  scope: user:read
slug: v12-scopes
source_filename: v12-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/v12-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/v12-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://v12.sh/oauth/authorize\n    tokenUrl: https://v12.sh/api/oauth/token\nscopes:\n- scope: findings:read\n  description: 'The inbox: findings, their status, reports and comments.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: findings:write\n  description: Change status, comment and update triage decisions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: repos:read\n  description: Repositories, branches, pull requests, tags and Steer instructions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: repos:write\n  description: Add public repositories to the workspace; owners can also add private repositories\n    granted by GitHub, create repositories V12 hosts and push\
  \ code to them.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: runs:manage\n  description: Cancel runs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: runs:read\n  description: Runs, their progress and context documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: runs:share\n  description: Create, change and revoke guest links that open a run to people outside the organization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: runs:write\n  description: Estimate and start runs; add or archive context documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope: steers:write\n  description: Create, edit, archive and restore Steers. Archiving detaches them from Autopilot\n    rules; finding tags and run history are kept.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n- scope:\
  \ user:read\n  description: 'The member directory: usernames, emails and roles. Any key reads its own account,\n    organization and credit balance without it.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/v12-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v12/refs/heads/main/scopes/v12-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Company
- Security
- DevOps
- Automation
- Code Analysis
token_bound: false
token_urls:
- https://v12.sh/api/oauth/token
---
