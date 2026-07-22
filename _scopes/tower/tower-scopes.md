---
api_specs:
- filename: tower-openapi-original.json
  format: json
  label: Tower API
  slug: tower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/openapi/tower-openapi-original.json
authorization_urls: []
description: Tower's documented permission-scope system for API keys (not OAuth — Tower's OpenAPI declares apiKey + bearer schemes, no oauth2 flows). Every API endpoint requires a scope, listed per-operation in the API reference under "Authorization"; API keys default to the creating account's role and can be minted with a reduced scope set via the create-api-key operation's `scopes` parameter. A key lacking the required scope receives 403 Forbidden. Captured verbatim from the "Available scopes" table. (The only OAuth-shaped surface is vend-catalog-credentials, which mints short-lived OAuth bearer tokens for Iceberg catalog access.)
docs: https://docs.tower.dev/docs/using-tower/api-keys
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tower Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tower publishes 53 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tower API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tower
provider_slug: tower
schemes: []
scope_count: 53
scope_names:
- api_keys
- api_keys:read
- api_keys:create
- api_keys:delete
- apps
- apps:read
- apps:run
- apps:deploy
- apps:create
- apps:update
- apps:delete
- catalogs
- catalogs:read
- catalogs:create
- catalogs:update
- catalogs:delete
- catalogs:export
- envs
- envs:create
- envs:read
- envs:update
- notifications
- notifications:read
- notifications:delete
- runs
- runs:read
- runs:cancel
- runs:logs
- runners
- runners:read
- runners:credentials:create
- sandbox
- sandbox:secrets:create
- schedules
- schedules:create
- schedules:read
- schedules:update
- schedules:delete
- secrets
- secrets:read
- secrets:create
- secrets:update
- secrets:delete
- teams
- teams:create
- teams:read
- teams:update
- teams:delete
- webhooks
- webhooks:read
- webhooks:create
- webhooks:update
- webhooks:delete
scopes:
- description: Access to all API key operations.
  flows: []
  scope: api_keys
- description: Read access for API keys.
  flows: []
  scope: api_keys:read
- description: Create access for API keys.
  flows: []
  scope: api_keys:create
- description: Delete access for API keys.
  flows: []
  scope: api_keys:delete
- description: Access to all apps operations.
  flows: []
  scope: apps
- description: Read access for apps.
  flows: []
  scope: apps:read
- description: Allows the API to run apps.
  flows: []
  scope: apps:run
- description: Allows the API key to be used to deploy a new app version.
  flows: []
  scope: apps:deploy
- description: Create access for apps.
  flows: []
  scope: apps:create
- description: Update access for apps (e.g. renaming app).
  flows: []
  scope: apps:update
- description: Delete access for apps.
  flows: []
  scope: apps:delete
- description: Access to all Tower catalog operations.
  flows: []
  scope: catalogs
- description: Read access for catalogs.
  flows: []
  scope: catalogs:read
- description: Create access for catalogs.
  flows: []
  scope: catalogs:create
- description: Update access for catalogs.
  flows: []
  scope: catalogs:update
- description: Delete access for catalogs.
  flows: []
  scope: catalogs:delete
- description: Export access for catalogs.
  flows: []
  scope: catalogs:export
- description: Access to all environment operations.
  flows: []
  scope: envs
- description: Create access for environments.
  flows: []
  scope: envs:create
- description: Read access for environments.
  flows: []
  scope: envs:read
- description: Update access for environments.
  flows: []
  scope: envs:update
- description: Access to all notification operations.
  flows: []
  scope: notifications
- description: Read access for notifications.
  flows: []
  scope: notifications:read
- description: Delete access for notifications.
  flows: []
  scope: notifications:delete
- description: Access to all run operations.
  flows: []
  scope: runs
- description: Read access for runs.
  flows: []
  scope: runs:read
- description: Allows for canceling an active run.
  flows: []
  scope: runs:cancel
- description: Read access for run logs, including the stream of logs.
  flows: []
  scope: runs:logs
- description: Access to all self-hosted runner operations.
  flows: []
  scope: runners
- description: Read access to runners.
  flows: []
  scope: runners:read
- description: Allows for creating credentials for self-hosted runners.
  flows: []
  scope: runners:credentials:create
- description: Access to all Tower sandbox operations.
  flows: []
  scope: sandbox
- description: Allows for creating a new secret in a sandbox.
  flows: []
  scope: sandbox:secrets:create
- description: Access to all schedules operations.
  flows: []
  scope: schedules
- description: Create access for schedules.
  flows: []
  scope: schedules:create
- description: Read access for schedules.
  flows: []
  scope: schedules:read
- description: Update access for schedules.
  flows: []
  scope: schedules:update
- description: Delete access for schedules.
  flows: []
  scope: schedules:delete
- description: Access to all secrets operations.
  flows: []
  scope: secrets
- description: Read access for secrets.
  flows: []
  scope: secrets:read
- description: Create access for secrets.
  flows: []
  scope: secrets:create
- description: Update access for secrets.
  flows: []
  scope: secrets:update
- description: Delete access for secrets.
  flows: []
  scope: secrets:delete
- description: Access to all team operations.
  flows: []
  scope: teams
- description: Create access for teams.
  flows: []
  scope: teams:create
- description: Read access for teams.
  flows: []
  scope: teams:read
- description: Update access for teams.
  flows: []
  scope: teams:update
- description: Delete access for teams.
  flows: []
  scope: teams:delete
- description: Access to all webhooks operations.
  flows: []
  scope: webhooks
- description: Read access for webhooks.
  flows: []
  scope: webhooks:read
- description: Create access for webhooks.
  flows: []
  scope: webhooks:create
- description: Update access for webhooks.
  flows: []
  scope: webhooks:update
- description: Delete access for webhooks.
  flows: []
  scope: webhooks:delete
slug: tower-scopes
source_filename: tower-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tower.dev/docs/using-tower/api-keys\ndocs: https://docs.tower.dev/docs/using-tower/api-keys\ndescription: >-\n  Tower's documented permission-scope system for API keys (not OAuth — Tower's\n  OpenAPI declares apiKey + bearer schemes, no oauth2 flows). Every API endpoint\n  requires a scope, listed per-operation in the API reference under\n  \"Authorization\"; API keys default to the creating account's role and can be\n  minted with a reduced scope set via the create-api-key operation's `scopes`\n  parameter. A key lacking the required scope receives 403 Forbidden. Captured\n  verbatim from the \"Available scopes\" table. (The only OAuth-shaped surface is\n  vend-catalog-credentials, which mints short-lived OAuth bearer tokens for\n  Iceberg catalog access.)\nscheme: api-key-scopes\nscopes:\n  - {scope: \"api_keys\", description: \"Access to all API key operations.\"}\n  - {scope: \"api_keys:read\", description:\
  \ \"Read access for API keys.\"}\n  - {scope: \"api_keys:create\", description: \"Create access for API keys.\"}\n  - {scope: \"api_keys:delete\", description: \"Delete access for API keys.\"}\n  - {scope: \"apps\", description: \"Access to all apps operations.\"}\n  - {scope: \"apps:read\", description: \"Read access for apps.\"}\n  - {scope: \"apps:run\", description: \"Allows the API to run apps.\"}\n  - {scope: \"apps:deploy\", description: \"Allows the API key to be used to deploy a new app version.\"}\n  - {scope: \"apps:create\", description: \"Create access for apps.\"}\n  - {scope: \"apps:update\", description: \"Update access for apps (e.g. renaming app).\"}\n  - {scope: \"apps:delete\", description: \"Delete access for apps.\"}\n  - {scope: \"catalogs\", description: \"Access to all Tower catalog operations.\"}\n  - {scope: \"catalogs:read\", description: \"Read access for catalogs.\"}\n  - {scope: \"catalogs:create\", description: \"Create access for catalogs.\"}\n  - {scope:\
  \ \"catalogs:update\", description: \"Update access for catalogs.\"}\n  - {scope: \"catalogs:delete\", description: \"Delete access for catalogs.\"}\n  - {scope: \"catalogs:export\", description: \"Export access for catalogs.\"}\n  - {scope: \"envs\", description: \"Access to all environment operations.\"}\n  - {scope: \"envs:create\", description: \"Create access for environments.\"}\n  - {scope: \"envs:read\", description: \"Read access for environments.\"}\n  - {scope: \"envs:update\", description: \"Update access for environments.\"}\n  - {scope: \"notifications\", description: \"Access to all notification operations.\"}\n  - {scope: \"notifications:read\", description: \"Read access for notifications.\"}\n  - {scope: \"notifications:delete\", description: \"Delete access for notifications.\"}\n  - {scope: \"runs\", description: \"Access to all run operations.\"}\n  - {scope: \"runs:read\", description: \"Read access for runs.\"}\n  - {scope: \"runs:cancel\", description: \"Allows\
  \ for canceling an active run.\"}\n  - {scope: \"runs:logs\", description: \"Read access for run logs, including the stream of logs.\"}\n  - {scope: \"runners\", description: \"Access to all self-hosted runner operations.\"}\n  - {scope: \"runners:read\", description: \"Read access to runners.\"}\n  - {scope: \"runners:credentials:create\", description: \"Allows for creating credentials for self-hosted runners.\"}\n  - {scope: \"sandbox\", description: \"Access to all Tower sandbox operations.\"}\n  - {scope: \"sandbox:secrets:create\", description: \"Allows for creating a new secret in a sandbox.\"}\n  - {scope: \"schedules\", description: \"Access to all schedules operations.\"}\n  - {scope: \"schedules:create\", description: \"Create access for schedules.\"}\n  - {scope: \"schedules:read\", description: \"Read access for schedules.\"}\n  - {scope: \"schedules:update\", description: \"Update access for schedules.\"}\n  - {scope: \"schedules:delete\", description: \"Delete access for\
  \ schedules.\"}\n  - {scope: \"secrets\", description: \"Access to all secrets operations.\"}\n  - {scope: \"secrets:read\", description: \"Read access for secrets.\"}\n  - {scope: \"secrets:create\", description: \"Create access for secrets.\"}\n  - {scope: \"secrets:update\", description: \"Update access for secrets.\"}\n  - {scope: \"secrets:delete\", description: \"Delete access for secrets.\"}\n  - {scope: \"teams\", description: \"Access to all team operations.\"}\n  - {scope: \"teams:create\", description: \"Create access for teams.\"}\n  - {scope: \"teams:read\", description: \"Read access for teams.\"}\n  - {scope: \"teams:update\", description: \"Update access for teams.\"}\n  - {scope: \"teams:delete\", description: \"Delete access for teams.\"}\n  - {scope: \"webhooks\", description: \"Access to all webhooks operations.\"}\n  - {scope: \"webhooks:read\", description: \"Read access for webhooks.\"}\n  - {scope: \"webhooks:create\", description: \"Create access for webhooks.\"\
  }\n  - {scope: \"webhooks:update\", description: \"Update access for webhooks.\"}\n  - {scope: \"webhooks:delete\", description: \"Delete access for webhooks.\"}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tower/refs/heads/main/scopes/tower-scopes.yml
summary_line: 53 scopes
tags:
- Data Infrastructure
- Data Engineering
- Python
- Apache Iceberg
- Lakehouse
- Orchestration
- Data Pipelines
- AI Agents
- MCP
- ETL
token_urls: []
---
