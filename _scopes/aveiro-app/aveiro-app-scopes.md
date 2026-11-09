---
api_specs:
- filename: aveiro-app-openapi-generated.yml
  format: yaml
  label: Aveiro API
  slug: aveiro-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aveiro-app/openapi/_ae-authored/aveiro-app-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Aveiro App Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aveiro publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aveiro API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aveiro
provider_slug: aveiro-app
schemes: []
scope_count: 12
scope_names:
- sites:read
- sites:write
- collections:write
- content:read
- content:write
- content:delete
- publish:write
- audience:write
- social:write
- social:approve
- newsletter:read
- newsletter:write
scopes:
- description: Read site metadata, pages, and content.
  flows: []
  scope: sites:read
- description: Create, edit, delete sites and pages.
  flows: []
  scope: sites:write
- description: Create, edit, delete collections.
  flows: []
  scope: collections:write
- description: Read content items.
  flows: []
  scope: content:read
- description: Create, edit, delete content items.
  flows: []
  scope: content:write
- description: Delete content items.
  flows: []
  scope: content:delete
- description: Publish sites and pages.
  flows: []
  scope: publish:write
- description: Manage audience lists and segments.
  flows: []
  scope: audience:write
- description: Create and edit social posts.
  flows: []
  scope: social:write
- description: Approve or reject social posts.
  flows: []
  scope: social:approve
- description: Read newsletters and subscriber lists.
  flows: []
  scope: newsletter:read
- description: Create, edit, delete newsletters and manage subscribers.
  flows: []
  scope: newsletter:write
slug: aveiro-app-scopes
source_filename: aveiro-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://api.aveiro.app/authentication\nscopes:\n  - name: sites:read\n    description: Read site metadata, pages, and content.\n  - name: sites:write\n    description: Create, edit, delete sites and pages.\n  - name: collections:write\n    description: Create, edit, delete collections.\n  - name: content:read\n    description: Read content items.\n  - name: content:write\n    description: Create, edit, delete content items.\n  - name: content:delete\n    description: Delete content items.\n  - name: publish:write\n    description: Publish sites and pages.\n  - name: audience:write\n    description: Manage audience lists and segments.\n  - name: social:write\n    description: Create and edit social posts.\n  - name: social:approve\n    description: Approve or reject social posts.\n  - name: newsletter:read\n    description: Read newsletters and subscriber lists.\n  - name: newsletter:write\n    description: Create, edit, delete\
  \ newsletters and manage subscribers.\n"
source_yaml_url: https://artifacts.apis.io/aveiro-app/scopes/aveiro-app-scopes.yml
summary_line: 12 scopes
tags:
- Company
- No-Code
- Publishing
- Templates
- Artificial Intelligence
token_bound: false
token_urls: []
---
