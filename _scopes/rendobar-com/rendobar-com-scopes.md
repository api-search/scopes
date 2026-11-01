---
api_specs:
- filename: rendobar-com-account-api-openapi.yml
  format: yaml
  label: rendobar-com Account API
  slug: rendobar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-account-api-openapi.yml
- filename: rendobar-com-api-keys-api-openapi.yml
  format: yaml
  label: rendobar-com API Keys API
  slug: rendobar-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-api-keys-api-openapi.yml
- filename: rendobar-com-assets-api-openapi.yml
  format: yaml
  label: rendobar-com Assets API
  slug: rendobar-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-assets-api-openapi.yml
- filename: rendobar-com-billing-api-openapi.yml
  format: yaml
  label: rendobar-com Billing API
  slug: rendobar-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-billing-api-openapi.yml
- filename: rendobar-com-compose-api-openapi.yml
  format: yaml
  label: rendobar-com Compose API
  slug: rendobar-com-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-compose-api-openapi.yml
- filename: rendobar-com-jobs-api-openapi.yml
  format: yaml
  label: rendobar-com Jobs API
  slug: rendobar-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-jobs-api-openapi.yml
- filename: rendobar-com-models-api-openapi.yml
  format: yaml
  label: rendobar-com Models API
  slug: rendobar-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-models-api-openapi.yml
- filename: rendobar-com-notifications-api-openapi.yml
  format: yaml
  label: rendobar-com Notifications API
  slug: rendobar-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-notifications-api-openapi.yml
- filename: rendobar-com-organizations-api-openapi.yml
  format: yaml
  label: rendobar-com Organizations API
  slug: rendobar-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-organizations-api-openapi.yml
- filename: rendobar-com-sharing-api-openapi.yml
  format: yaml
  label: rendobar-com Sharing API
  slug: rendobar-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-sharing-api-openapi.yml
- filename: rendobar-com-storage-api-openapi.yml
  format: yaml
  label: rendobar-com Storage API
  slug: rendobar-com-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-storage-api-openapi.yml
- filename: rendobar-com-team-api-openapi.yml
  format: yaml
  label: rendobar-com Team API
  slug: rendobar-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-team-api-openapi.yml
- filename: rendobar-com-upload-sessions-api-openapi.yml
  format: yaml
  label: rendobar-com Upload Sessions API
  slug: rendobar-com-upload-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-upload-sessions-api-openapi.yml
- filename: rendobar-com-webhooks-api-openapi.yml
  format: yaml
  label: rendobar-com Webhooks API
  slug: rendobar-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rendobar Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'rendobar-com publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the rendobar-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: rendobar-com
provider_slug: rendobar-com
schemes: []
scope_count: 14
scope_names:
- jobs:read
- jobs:write
- assets:read
- assets:write
- webhooks:read
- webhooks:write
- billing:read
- billing:write
- orgs:read
- orgs:write
- keys:read
- keys:write
- storage:read
- storage:write
scopes:
- description: See your jobs and their results
  flows: []
  scope: jobs:read
- description: Run jobs, which spends credits
  flows: []
  scope: jobs:write
- description: See and download your files
  flows: []
  scope: assets:read
- description: Upload and delete files
  flows: []
  scope: assets:write
- description: See where your events are delivered
  flows: []
  scope: webhooks:read
- description: Manage where your events are delivered
  flows: []
  scope: webhooks:write
- description: See your plan, balance and usage
  flows: []
  scope: billing:read
- description: Change your plan and payment methods
  flows: []
  scope: billing:write
- description: See your organization and its members
  flows: []
  scope: orgs:read
- description: Manage your organization and its members
  flows: []
  scope: orgs:write
- description: See which API keys exist
  flows: []
  scope: keys:read
- description: Create and revoke API keys
  flows: []
  scope: keys:write
- description: See which storage connections exist
  flows: []
  scope: storage:read
- description: Connect, rotate and remove storage connections
  flows: []
  scope: storage:write
slug: rendobar-com-scopes
source_filename: rendobar-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://rendobar.com/docs/concepts/scopes.md\nscopes:\n  - name: jobs:read\n    description: See your jobs and their results\n  - name: jobs:write\n    description: Run jobs, which spends credits\n  - name: assets:read\n    description: See and download your files\n  - name: assets:write\n    description: Upload and delete files\n  - name: webhooks:read\n    description: See where your events are delivered\n  - name: webhooks:write\n    description: Manage where your events are delivered\n  - name: billing:read\n    description: See your plan, balance and usage\n  - name: billing:write\n    description: Change your plan and payment methods\n  - name: orgs:read\n    description: See your organization and its members\n  - name: orgs:write\n    description: Manage your organization and its members\n  - name: keys:read\n    description: See which API keys exist\n  - name: keys:write\n    description: Create and revoke API keys\n\
  \  - name: storage:read\n    description: See which storage connections exist\n  - name: storage:write\n    description: Connect, rotate and remove storage connections\n"
source_yaml_url: https://artifacts.apis.io/rendobar-com/scopes/rendobar-com-scopes.yml
summary_line: 14 scopes
tags:
- Company
- VideoProcessing
- FFmpeg
- AI
- Serverless
- MediaAPI
token_bound: false
token_urls: []
---
