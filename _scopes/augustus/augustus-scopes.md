---
api_specs:
- filename: augustus-openapi-original.yml
  format: yaml
  label: Augustus Banking API
  slug: augustus-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.augustus.com/v1/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Augustus Scopes
name_suffix: OAuth Scopes
note: Augustus does not use OAuth. Scopes gate scoped bearer API keys (not OAuth access tokens). Every API key carries one or more scopes of the shape resource:action, enforced on every request. GET /v1/scopes is the live, public (no-auth) source of truth, filtered by the request's api-version header. A 403 insufficient_scope response carries a required_scopes array.
overview: 'Augustus publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Augustus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Augustus
provider_slug: augustus
schemes: []
scope_count: 16
scope_names:
- payouts:read
- payouts:write
- deposits:read
- returns:read
- returns:write
- conversions:read
- conversions:write
- quotes:read
- accounts:read
- accounts:write
- account_programs:read
- webhook_subscriptions:read
- webhook_subscriptions:write
- events:read
- webhook_deliveries:read
- webhook_deliveries:write
scopes:
- description: View payouts and their status
  flows: []
  scope: payouts:read
- description: Initiate and manage payouts
  flows: []
  scope: payouts:write
- description: View deposits
  flows: []
  scope: deposits:read
- description: View deposit returns
  flows: []
  scope: returns:read
- description: Initiate deposit returns
  flows: []
  scope: returns:write
- description: View FX conversions
  flows: []
  scope: conversions:read
- description: Initiate FX conversions
  flows: []
  scope: conversions:write
- description: View FX quotes (persisted and indicative)
  flows: []
  scope: quotes:read
- description: View accounts and holders
  flows: []
  scope: accounts:read
- description: Create and manage accounts
  flows: []
  scope: accounts:write
- description: View account programs and their lifecycle status
  flows: []
  scope: account_programs:read
- description: View webhook subscriptions
  flows: []
  scope: webhook_subscriptions:read
- description: Create, modify, and delete webhook subscriptions; send test events
  flows: []
  scope: webhook_subscriptions:write
- description: View webhook events and their payloads
  flows: []
  scope: events:read
- description: View webhook delivery history and outcomes
  flows: []
  scope: webhook_deliveries:read
- description: Redeliver webhook deliveries
  flows: []
  scope: webhook_deliveries:write
slug: augustus-scopes
source_filename: augustus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.augustus.com/v1/scopes\ndocs: https://docs.augustus.com/v1/scopes\nnote: >-\n  Augustus does not use OAuth. Scopes gate scoped bearer API keys (not OAuth\n  access tokens). Every API key carries one or more scopes of the shape\n  resource:action, enforced on every request. GET /v1/scopes is the live,\n  public (no-auth) source of truth, filtered by the request's api-version\n  header. A 403 insufficient_scope response carries a required_scopes array.\ncatalogue_endpoint: GET /v1/scopes\nscope_shape: 'resource:action'\nactions:\n- read\n- write\nscopes:\n- scope: payouts:read\n  description: View payouts and their status\n- scope: payouts:write\n  description: Initiate and manage payouts\n- scope: deposits:read\n  description: View deposits\n- scope: returns:read\n  description: View deposit returns\n- scope: returns:write\n  description: Initiate deposit returns\n- scope: conversions:read\n  description: View FX\
  \ conversions\n- scope: conversions:write\n  description: Initiate FX conversions\n- scope: quotes:read\n  description: View FX quotes (persisted and indicative)\n- scope: accounts:read\n  description: View accounts and holders\n- scope: accounts:write\n  description: Create and manage accounts\n- scope: account_programs:read\n  description: View account programs and their lifecycle status\n- scope: webhook_subscriptions:read\n  description: View webhook subscriptions\n- scope: webhook_subscriptions:write\n  description: Create, modify, and delete webhook subscriptions; send test events\n- scope: events:read\n  description: View webhook events and their payloads\n- scope: webhook_deliveries:read\n  description: View webhook delivery history and outcomes\n- scope: webhook_deliveries:write\n  description: Redeliver webhook deliveries\naliases:\n- alias: full_access\n  expands_to: Every scope in the catalogue (auto-gains scopes added later)\n- alias: read_only\n  expands_to: Every :read scope\n\
  - alias: '*:read'\n  expands_to: Every :read scope\n- alias: '<resource>:*'\n  expands_to: Every action for a resource (e.g. payouts:*)\nrecommended_sets:\n- use_case: Server-side payouts integration\n  scopes: payouts:* events:read webhook_subscriptions:write webhook_deliveries:read\n- use_case: Read-only BI / analytics\n  scopes: read_only\n- use_case: Webhook receiver only\n  scopes: events:read webhook_deliveries:*\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/scopes/augustus-scopes.yml
summary_line: 16 scopes
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Stablecoin
- Payouts
- Foreign Exchange
- Webhooks
token_urls: []
---
