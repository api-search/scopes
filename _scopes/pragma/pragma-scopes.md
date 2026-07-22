---
authorization_urls: []
description: ''
docs: https://docs.firstlook.gg/developers/api/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Pragma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pragma publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pragma API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pragma
provider_slug: pragma
schemes:
- name: FirstLookApiToken
  source: https://docs.firstlook.gg/developers/api/
  type: apiKey
scope_count: 5
scope_names:
- players.query
- players.lookup
- analytics.events.write
- surveys.read
- creators.read
scopes:
- description: Search players with filters.
  flows: []
  scope: players.query
- description: Fetch a single player, or find-or-create a player.
  flows: []
  scope: players.lookup
- description: Record analytics events — send sessions, counters, and durations (requires the Retention feature).
  flows: []
  scope: analytics.events.write
- description: List and export surveys.
  flows: []
  scope: surveys.read
- description: Search creators and read the public creator leaderboard.
  flows: []
  scope: creators.read
slug: pragma-scopes
source_filename: pragma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.firstlook.gg/developers/api/\ndocs: https://docs.firstlook.gg/developers/api/\nnotes: >-\n  FirstLook External API tokens are scoped: each token is granted one or more of\n  the permission categories below at creation time (Settings -> Developer). These\n  are the documented scope groups; the exact machine scope strings are enumerated\n  in the Swagger UI at https://api.firstlook.gg/external/swagger-ui/.\nschemes:\n  - name: FirstLookApiToken\n    type: apiKey\n    source: https://docs.firstlook.gg/developers/api/\nscopes:\n  - scope: players.query\n    description: Search players with filters.\n    sources: [https://docs.firstlook.gg/developers/api/]\n  - scope: players.lookup\n    description: Fetch a single player, or find-or-create a player.\n    sources: [https://docs.firstlook.gg/developers/api/]\n  - scope: analytics.events.write\n    description: Record analytics events — send sessions, counters, and durations\
  \ (requires the Retention feature).\n    sources: [https://docs.firstlook.gg/developers/api/]\n  - scope: surveys.read\n    description: List and export surveys.\n    sources: [https://docs.firstlook.gg/developers/api/]\n  - scope: creators.read\n    description: Search creators and read the public creator leaderboard.\n    sources: [https://docs.firstlook.gg/developers/api/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pragma/refs/heads/main/scopes/pragma-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Infrastructure
- Gaming
- Game Backend
- Live Operations
- Player Accounts
- Authentication
- Commerce
- Playtesting
- Community
- Analytics
- Developer Tools
token_urls: []
---
