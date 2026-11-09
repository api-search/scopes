---
api_specs:
- filename: api.json
  format: json
  label: Vocenya API
  slug: vocenya-api
  spec_type: OpenAPI
  url: https://vocenya.com/docs/api.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Vocenya Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'vocenya-com publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the vocenya-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: vocenya-com
provider_slug: vocenya-com
schemes: []
scope_count: 11
scope_names:
- calls:read
- leads:read
- leads:write
- bookings:read
- outbound:read
- outbound:write
- dnc:read
- dnc:write
- chats:read
- chats:write
- webhooks:manage
scopes:
- description: Read calls
  flows: []
  scope: calls:read
- description: Read leads
  flows: []
  scope: leads:read
- description: Create leads
  flows: []
  scope: leads:write
- description: Read bookings
  flows: []
  scope: bookings:read
- description: Read outbound AI calls
  flows: []
  scope: outbound:read
- description: Queue outbound AI calls and check their status
  flows: []
  scope: outbound:write
- description: Read the Do Not Call list
  flows: []
  scope: dnc:read
- description: Add to and remove from the Do Not Call list
  flows: []
  scope: dnc:write
- description: Read website chats
  flows: []
  scope: chats:read
- description: Reply to and close website chats
  flows: []
  scope: chats:write
- description: Manage webhooks
  flows: []
  scope: webhooks:manage
slug: vocenya-com-scopes
source_filename: vocenya-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://vocenya.com/docs/authentication\nscopes:\n  - name: calls:read\n    description: Read calls\n  - name: leads:read\n    description: Read leads\n  - name: leads:write\n    description: Create leads\n  - name: bookings:read\n    description: Read bookings\n  - name: outbound:read\n    description: Read outbound AI calls\n  - name: outbound:write\n    description: Queue outbound AI calls and check their status\n  - name: dnc:read\n    description: Read the Do Not Call list\n  - name: dnc:write\n    description: Add to and remove from the Do Not Call list\n  - name: chats:read\n    description: Read website chats\n  - name: chats:write\n    description: Reply to and close website chats\n  - name: webhooks:manage\n    description: Manage webhooks\n"
source_yaml_url: https://artifacts.apis.io/vocenya-com/scopes/vocenya-com-scopes.yml
summary_line: 11 scopes
tags:
- Artificial Intelligence
- Communications
- Customer Service
- Automation
- Voice
token_bound: false
token_urls: []
---
