---
api_specs:
- filename: therankingfactory-com-public-api-openapi.yml
  format: yaml
  label: therankingfactory-com Public API
  slug: therankingfactory-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/therankingfactory-com/openapi/therankingfactory-com-public-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Therankingfactory Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'therankingfactory-com publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the therankingfactory-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: therankingfactory-com
provider_slug: therankingfactory-com
schemes: []
scope_count: 6
scope_names:
- visibility:read
- gaps:read
- evidence:read
- entity:read
- recommendations:read
- write
scopes:
- description: 'Read AI-visibility measurements: runs, per-engine rates, per-topic history.'
  flows: []
  scope: visibility:read
- description: 'Read the evidence-gap list: what is open, in flight, closed, abandoned, and waiting on a person.'
  flows: []
  scope: gaps:read
- description: 'Read the published-evidence ledger: what was published where, when, and what AI answers cited.'
  flows: []
  scope: evidence:read
- description: 'Read the business itself: its identity, the facts asserted about it, and the sources behind them.'
  flows: []
  scope: entity:read
- description: 'Read the project reviewer''s recommendations: what it suggests changing, with the figures it measured. Reading only; nothing is applied.'
  flows: []
  scope: recommendations:read
- description: 'Make changes when you ask it to: correct the business''s entity details, say what one of its products is, ask the Evidence Engine to work a gap now, approve a page or a held Google file that is waiting for you, spread held Google files over the coming days, and start a visibility run on your AI keys. Each change goes through the same checks as the app and is recorded under Settings → Advanced → Agent access. Without this, it can only read.'
  flows: []
  scope: write
slug: therankingfactory-com-scopes
source_filename: therankingfactory-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://therankingfactory.com/.well-known/mcp/server-card.json\nscopes:\n  - scope: visibility:read\n    description: \"Read AI-visibility measurements: runs, per-engine rates, per-topic history.\"\n  - scope: gaps:read\n    description: \"Read the evidence-gap list: what is open, in flight, closed, abandoned, and waiting on a person.\"\n  - scope: evidence:read\n    description: \"Read the published-evidence ledger: what was published where, when, and what AI answers cited.\"\n  - scope: entity:read\n    description: \"Read the business itself: its identity, the facts asserted about it, and the sources behind them.\"\n  - scope: recommendations:read\n    description: \"Read the project reviewer's recommendations: what it suggests changing, with the figures it measured. Reading only; nothing is applied.\"\n  - scope: write\n    description: \"Make changes when you ask it to: correct the business's entity details, say what one\
  \ of its products is, ask the Evidence Engine to work a gap now, approve a page or a held Google file that is waiting for you, spread held Google files over the coming days, and start a visibility run on your AI keys. Each change goes through the same checks as the app and is recorded under Settings → Advanced → Agent access. Without this, it can only read.\"\n"
source_yaml_url: https://artifacts.apis.io/therankingfactory-com/scopes/therankingfactory-com-scopes.yml
summary_line: 6 scopes
tags:
- AI
- SEO
- Marketing
- Analytics
- Automation
token_bound: false
token_urls: []
---
