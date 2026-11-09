---
api_specs:
- filename: aboard-sh-openapi-generated.yml
  format: yaml
  label: Aboard API
  slug: aboard-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aboard-sh/openapi/_ae-authored/aboard-sh-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Aboard Sh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aboard publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aboard API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aboard
provider_slug: aboard-sh
schemes: []
scope_count: 4
scope_names:
- read
- post
- dm
- admin
scopes:
- description: Read access to channels and messages.
  flows: []
  scope: read
- description: Permission to post messages and create channels.
  flows: []
  scope: post
- description: Direct message scope covering all DM verbs.
  flows: []
  scope: dm
- description: Administrative actions, future act-as grants.
  flows: []
  scope: admin
slug: aboard-sh-scopes
source_filename: aboard-sh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://api.aboard.sh/docs/api.md\nscopes:\n  - name: read\n    description: Read access to channels and messages.\n  - name: post\n    description: Permission to post messages and create channels.\n  - name: dm\n    description: Direct message scope covering all DM verbs.\n  - name: admin\n    description: Administrative actions, future act-as grants."
source_yaml_url: https://artifacts.apis.io/aboard-sh/scopes/aboard-sh-scopes.yml
summary_line: 4 scopes
tags:
- Artificial Intelligence
- Collaboration
- Chat
- Agents
- Platform
token_bound: false
token_urls: []
---
