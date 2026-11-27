---
authorization_urls: []
description: ''
docs: https://cornelius.bot/teams
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cornelius Scopes
name_suffix: OAuth Scopes
note: These are OIDC identity scopes only; the docs name no per-tool or resource scopes. Tool access (six read, one write) is fixed, not scope-gated.
overview: 'Cornelius publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cornelius API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cornelius
provider_slug: cornelius-bot
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in (member identity).
  flows: []
  scope: openid
- description: Member identity.
  flows: []
  scope: profile
- description: Member email address.
  flows: []
  scope: email
- description: Refresh token so the member stays connected.
  flows: []
  scope: offline_access
slug: cornelius-bot-scopes
source_filename: cornelius-bot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cornelius.bot/teams\ndocs: https://cornelius.bot/teams\nname: Cornelius OAuth scopes\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (member identity).\n- name: profile\n  description: Member identity.\n- name: email\n  description: Member email address.\n- name: offline_access\n  description: Refresh token so the member stays connected.\nevidence: \"The requested scopes are openid profile email offline_access : the member's identity and email, plus a refresh token so they stay connected.\"\nnote: These are OIDC identity scopes only; the docs name no per-tool or resource scopes. Tool access (six read, one write) is fixed, not scope-gated.\n"
source_yaml_url: https://artifacts.apis.io/cornelius-bot/scopes/cornelius-bot-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Personal Assistant
- MCP
- Knowledge Graph
- Productivity
token_bound: false
token_urls: []
---
