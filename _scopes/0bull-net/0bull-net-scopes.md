---
api_specs:
- filename: 0bull-net-openapi-generated.yml
  format: yaml
  label: 0bull API
  slug: 0bull-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0bull-net/openapi/_ae-authored/0bull-net-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: 0Bull Net Scopes
name_suffix: OAuth Scopes
note: ''
overview: '0bull publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the 0bull API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 0bull
provider_slug: 0bull-net
schemes: []
scope_count: 5
scope_names:
- phones:read
- phones:control
- accounts
- submissions
- billing
scopes:
- description: List phones, view snapshots and on-screen text, and check run status.
  flows: []
  scope: phones:read
- description: Send input, commands, macros and agent runs to a phone.
  flows: []
  scope: phones:control
- description: Link, list, update and remove posting accounts.
  flows: []
  scope: accounts
- description: Create, list and cancel video submissions.
  flows: []
  scope: submissions
- description: View billing and request phone rentals or count changes.
  flows: []
  scope: billing
slug: 0bull-net-scopes
source_filename: 0bull-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource:\n  - https://docs.0bull.net/api.md\nscopes:\n  - name: \"phones:read\"\n    description: \"List phones, view snapshots and on-screen text, and check run status.\"\n  - name: \"phones:control\"\n    description: \"Send input, commands, macros and agent runs to a phone.\"\n  - name: \"accounts\"\n    description: \"Link, list, update and remove posting accounts.\"\n  - name: \"submissions\"\n    description: \"Create, list and cancel video submissions.\"\n  - name: \"billing\"\n    description: \"View billing and request phone rentals or count changes.\"\n"
source_yaml_url: https://artifacts.apis.io/0bull-net/scopes/0bull-net-scopes.yml
summary_line: 5 scopes
tags:
- iPhone
- Rentals
- Social Media
- Automation
token_bound: false
token_urls: []
---
