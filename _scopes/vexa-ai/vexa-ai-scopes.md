---
api_specs:
- filename: vexa-ai-openapi-generated.yml
  format: yaml
  label: vexa-ai API
  slug: vexa-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vexa-ai/openapi/_ae-authored/vexa-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Vexa Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'vexa-ai publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the vexa-ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: vexa-ai
provider_slug: vexa-ai
schemes: []
scope_count: 3
scope_names:
- bot
- tx
- browser
scopes:
- description: bot lifecycle — POST/GET/DELETE /bots, /bots/status, bot config and calendar connections.
  flows: []
  scope: bot
- description: transcript and meeting-record plane — /meetings*, /transcripts/*.
  flows: []
  scope: tx
- description: browser-tool capabilities; reaches no API route today.
  flows: []
  scope: browser
slug: vexa-ai-scopes
source_filename: vexa-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.vexa.ai/authentication.md\nscopes:\n  - name: bot\n    description: bot lifecycle — POST/GET/DELETE /bots, /bots/status, bot config and calendar connections.\n  - name: tx\n    description: transcript and meeting-record plane — /meetings*, /transcripts/*.\n  - name: browser\n    description: browser-tool capabilities; reaches no API route today.\n"
source_yaml_url: https://artifacts.apis.io/vexa-ai/scopes/vexa-ai-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Artificial Intelligence
- MeetingBot
- Transcription
- Open Source
- Self-Hosted
token_bound: false
token_urls: []
---
