---
api_specs:
- filename: fieldguide-openapi-original.json
  format: json
  label: Fieldguide API
  slug: fieldguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-openapi-original.json
authorization_urls: []
description: ''
docs: https://api.fieldguide.io/api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fieldguide Scopes
name_suffix: OAuth Scopes
note: Fieldguide authenticates with bearer API tokens (JWT); each token is granted a set of resource-level scopes of the form `<resource>:read` / `<resource>:write`. The live, unauthenticated /v1/scopes endpoint returns the authoritative scope registry captured verbatim below. This is an API-token permission model, not an OAuth 2.0 authorization-server flow — no oauth2 securityScheme is declared in the OpenAPI (auth is http bearer JWT).
overview: 'Fieldguide publishes 21 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fieldguide API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fieldguide
provider_slug: fieldguide
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  source: openapi/fieldguide-openapi-original.json
  type: http
scope_count: 21
scope_names:
- comments:read
- comments:write
- companies:read
- companies:write
- controls:read
- engagements.files:read
- engagements.files:write
- engagements:read
- engagements:write
- files:read
- insights:read
- milestones:read
- requests.files:read
- requests.files:write
- requests:read
- requests:write
- sheets:read
- sheets:write
- users:read
- webhooks:read
- webhooks:write
scopes:
- description: Can fetch information about Comments that I have access to
  flows: []
  scope: comments:read
- description: Can create/update Comments that I have access to
  flows: []
  scope: comments:write
- description: Can fetch information about Companies that I have access to
  flows: []
  scope: companies:read
- description: Can create/update Companies that I have access to
  flows: []
  scope: companies:write
- description: Can fetch information about Controls that I have access to
  flows: []
  scope: controls:read
- description: Can fetch information about Files & Folders in Engagements that I have access to
  flows: []
  scope: engagements.files:read
- description: Can create and update Files & Folders in Engagements that I have access to
  flows: []
  scope: engagements.files:write
- description: Can fetch information about Engagements that I have access to
  flows: []
  scope: engagements:read
- description: Can create/update Engagements that I have access to
  flows: []
  scope: engagements:write
- description: Can fetch information about Files that I have access to
  flows: []
  scope: files:read
- description: Can fetch information about Insights that I have access to
  flows: []
  scope: insights:read
- description: Can fetch information about Milestones that I have access to
  flows: []
  scope: milestones:read
- description: Can fetch information about Files from Requests that I have access to
  flows: []
  scope: requests.files:read
- description: Can upload Files to Requests that I have access to
  flows: []
  scope: requests.files:write
- description: Can fetch information about Requests that I have access to
  flows: []
  scope: requests:read
- description: Can create/update Requests that I have access to
  flows: []
  scope: requests:write
- description: Can read Sheet-related data that I have access to
  flows: []
  scope: sheets:read
- description: Can update Sheet-related data that I have access to
  flows: []
  scope: sheets:write
- description: Can fetch information about Users that I have access to
  flows: []
  scope: users:read
- description: Can fetch information about webhook subscriptions that I have created
  flows: []
  scope: webhooks:read
- description: Can create/update webhook subscriptions for my user
  flows: []
  scope: webhooks:write
slug: fieldguide-scopes
source_filename: fieldguide-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.fieldguide.io/v1/scopes\ndocs: https://api.fieldguide.io/api\nnote: >-\n  Fieldguide authenticates with bearer API tokens (JWT); each token is granted\n  a set of resource-level scopes of the form `<resource>:read` / `<resource>:write`.\n  The live, unauthenticated /v1/scopes endpoint returns the authoritative scope\n  registry captured verbatim below. This is an API-token permission model, not an\n  OAuth 2.0 authorization-server flow — no oauth2 securityScheme is declared in\n  the OpenAPI (auth is http bearer JWT).\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  source: openapi/fieldguide-openapi-original.json\nscopes:\n- scope: comments:read\n  resource: comments\n  description: Can fetch information about Comments that I have access to\n- scope: comments:write\n  resource: comments\n  description: Can create/update Comments that I have access to\n- scope: companies:read\n \
  \ resource: companies\n  description: Can fetch information about Companies that I have access to\n- scope: companies:write\n  resource: companies\n  description: Can create/update Companies that I have access to\n- scope: controls:read\n  resource: controls\n  description: Can fetch information about Controls that I have access to\n- scope: engagements.files:read\n  resource: engagements\n  description: Can fetch information about Files & Folders in Engagements that I have access to\n- scope: engagements.files:write\n  resource: engagements\n  description: Can create and update Files & Folders in Engagements that I have access to\n- scope: engagements:read\n  resource: engagements\n  description: Can fetch information about Engagements that I have access to\n- scope: engagements:write\n  resource: engagements\n  description: Can create/update Engagements that I have access to\n- scope: files:read\n  resource: files\n  description: Can fetch information about Files that I have access to\n\
  - scope: insights:read\n  resource: insights\n  description: Can fetch information about Insights that I have access to\n- scope: milestones:read\n  resource: milestones\n  description: Can fetch information about Milestones that I have access to\n- scope: requests.files:read\n  resource: requests\n  description: Can fetch information about Files from Requests that I have access to\n- scope: requests.files:write\n  resource: requests\n  description: Can upload Files to Requests that I have access to\n- scope: requests:read\n  resource: requests\n  description: Can fetch information about Requests that I have access to\n- scope: requests:write\n  resource: requests\n  description: Can create/update Requests that I have access to\n- scope: sheets:read\n  resource: sheets\n  description: Can read Sheet-related data that I have access to\n- scope: sheets:write\n  resource: sheets\n  description: Can update Sheet-related data that I have access to\n- scope: users:read\n  resource: users\n \
  \ description: Can fetch information about Users that I have access to\n- scope: webhooks:read\n  resource: webhooks\n  description: Can fetch information about webhook subscriptions that I have created\n- scope: webhooks:write\n  resource: webhooks\n  description: Can create/update webhook subscriptions for my user\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/scopes/fieldguide-scopes.yml
summary_line: 21 scopes
tags:
- Company
- Audit
- Advisory
- Accounting
- Compliance
- Risk
- Engagement Management
- Artificial Intelligence
- Agents
- Webhooks
token_urls: []
---
