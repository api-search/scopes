---
authorization_urls: []
description: ''
docs: https://developers.crossbeam.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Crossbeam Scopes
name_suffix: OAuth Scopes
note: Crossbeam Partner API OAuth 2.0 scopes. Each endpoint's per-endpoint doc page states the scope it requires. Request `openid` at minimum plus the scope(s) for the endpoints you need.
overview: 'Crossbeam publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crossbeam API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Crossbeam
provider_slug: crossbeam
schemes:
- authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com
  flow: authorizationCode
  name: OAuth2
  tokenUrl: https://auth.crossbeam.com/oauth/token
scope_count: 6
scope_names:
- openid
- read:partnerships
- read:reports
- read:populations
- write:activity-timeline
- offline_access
scopes:
- description: Required baseline scope for all tokens.
  flows:
  - authorizationCode
  scope: openid
- description: Read partner data (e.g. GET /v1/partners — coverage, partner records).
  flows:
  - authorizationCode
  scope: read:partnerships
- description: Read report data (overlap / account-mapping results).
  flows:
  - authorizationCode
  scope: read:reports
- description: Read your populations.
  flows:
  - authorizationCode
  scope: read:populations
- description: Write activity onto the Crossbeam timeline. The only write path in the public API.
  flows:
  - authorizationCode
  scope: write:activity-timeline
- description: Issues a refresh token, needed for long-running apps (24h access-token lifetime).
  flows:
  - authorizationCode
  scope: offline_access
slug: crossbeam-scopes
source_filename: crossbeam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.crossbeam.com/\ndocs: https://developers.crossbeam.com/\nnote: >-\n  Crossbeam Partner API OAuth 2.0 scopes. Each endpoint's per-endpoint doc page states the\n  scope it requires. Request `openid` at minimum plus the scope(s) for the endpoints you need.\nschemes:\n  - name: OAuth2\n    flow: authorizationCode\n    authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com\n    tokenUrl: https://auth.crossbeam.com/oauth/token\nscopes:\n  - scope: openid\n    description: Required baseline scope for all tokens.\n    flows: [authorizationCode]\n  - scope: read:partnerships\n    description: Read partner data (e.g. GET /v1/partners — coverage, partner records).\n    flows: [authorizationCode]\n  - scope: read:reports\n    description: Read report data (overlap / account-mapping results).\n    flows: [authorizationCode]\n  - scope: read:populations\n    description: Read your\
  \ populations.\n    flows: [authorizationCode]\n  - scope: write:activity-timeline\n    description: Write activity onto the Crossbeam timeline. The only write path in the public API.\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issues a refresh token, needed for long-running apps (24h access-token lifetime).\n    flows: [authorizationCode]\nexample_scope_string: openid read:partnerships offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossbeam/refs/heads/main/scopes/crossbeam-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Ecosystem-Led Growth
- Partnerships
- Account Mapping
- Co-Selling
- Data Collaboration
- Sales Intelligence
- CRM
- Webhooks
- MCP
token_urls: []
---
