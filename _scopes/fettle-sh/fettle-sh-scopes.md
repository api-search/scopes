---
api_specs:
- filename: fettle-sh-api-openapi.json
  format: json
  label: fettle.sh Api API
  slug: fettle-sh-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fettle-sh/openapi/_original/fettle-sh-api-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fettle Sh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'fettle-sh publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the fettle-sh API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: fettle-sh
provider_slug: fettle-sh
schemes: []
scope_count: 2
scope_names:
- read
- write
scopes:
- description: List and inspect monitors, incidents, heartbeats and status pages.
  flows: []
  scope: read
- description: All read capabilities plus creating, changing, pausing and deleting resources.
  flows: []
  scope: write
slug: fettle-sh-scopes
source_filename: fettle-sh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://fettle.sh/docs/api-keys\nscopes:\n  - name: read\n    description: List and inspect monitors, incidents, heartbeats and status pages.\n  - name: write\n    description: All read capabilities plus creating, changing, pausing and deleting resources.\n"
source_yaml_url: https://artifacts.apis.io/fettle-sh/scopes/fettle-sh-scopes.yml
summary_line: 2 scopes
tags:
- Monitoring
- Uptime
- Developers
- AI Agents
token_bound: false
token_urls: []
---
