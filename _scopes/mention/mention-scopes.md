---
api_specs:
- filename: mention-accounts-api-openapi.yml
  format: yaml
  label: Mention Accounts API
  slug: mention-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-accounts-api-openapi.yml
- filename: mention-alerts-api-openapi.yml
  format: yaml
  label: Mention Alerts API
  slug: mention-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-alerts-api-openapi.yml
- filename: mention-authors-api-openapi.yml
  format: yaml
  label: Mention Authors API
  slug: mention-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-authors-api-openapi.yml
- filename: mention-mentions-api-openapi.yml
  format: yaml
  label: Mention Mentions API
  slug: mention-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-mentions-api-openapi.yml
- filename: mention-shares-api-openapi.yml
  format: yaml
  label: Mention Shares API
  slug: mention-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-shares-api-openapi.yml
- filename: mention-stats-api-openapi.yml
  format: yaml
  label: Mention Stats API
  slug: mention-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-stats-api-openapi.yml
- filename: mention-tags-api-openapi.yml
  format: yaml
  label: Mention Tags API
  slug: mention-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tags-api-openapi.yml
- filename: mention-tasks-api-openapi.yml
  format: yaml
  label: Mention Tasks API
  slug: mention-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tasks-api-openapi.yml
- filename: mention-app-api-openapi.yml
  format: yaml
  label: Mention App API
  slug: mention-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-app-api-openapi.yml
authorization_urls:
- https://web.mention.com/authorize
description: ''
docs: https://dev.mention.com/current/src/appendix/OAuth2.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mention Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mention uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://web.mention.net/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mention
provider_slug: mention
schemes:
- docs: https://dev.mention.com/current/src/appendix/OAuth2.html
  flows:
  - authorizationUrl: https://web.mention.com/authorize
    flow: authorizationCode
    scopes: {}
    tokenUrl: https://web.mention.net/oauth/v2/token
  name: oauth2
  note: 'Neither parameter list includes scope. The token response is {"access_token": "...", "token_type": "bearer"} with no scope member.'
  request_parameters:
    authorize:
    - client_id
    - redirect_uri
    - response_type
    token:
    - client_id
    - client_secret
    - redirect_uri
    - response_type
    - code
    - grant_type
  source: openapi/_original/mention-openapi.yml
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: mention-scopes
source_filename: mention-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/mention-openapi.yml\ndocs: https://dev.mention.com/current/src/appendix/OAuth2.html\nscope_count: 0\nsummary: >-\n  Mention runs an OAuth 2.0 authorization-code flow but defines NO scopes. There is no scope\n  parameter on the authorize request, no scopes list in the token response, and no permissions or\n  scopes reference page anywhere in the documentation. A granted token carries full access to the\n  authorizing account — the same access the account's own token has. This file records that as a\n  measured zero rather than omitting the artifact.\nschemes:\n  - name: oauth2\n    type: oauth2\n    source: openapi/_original/mention-openapi.yml\n    docs: https://dev.mention.com/current/src/appendix/OAuth2.html\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://web.mention.com/authorize\n        tokenUrl: https://web.mention.net/oauth/v2/token\n        scopes: {}\n    request_parameters:\n\
  \      authorize: [client_id, redirect_uri, response_type]\n      token: [client_id, client_secret, redirect_uri, response_type, code, grant_type]\n    note: >-\n      Neither parameter list includes scope. The token response is\n      {\"access_token\": \"...\", \"token_type\": \"bearer\"} with no scope member.\nscopes: []\nauthorization_model:\n  granularity: account\n  note: >-\n    Authorization in Mention is expressed through resources, not scopes. The Share object decides\n    which accounts can see which alert and carries a per-share permissions map (edit, delete) and a\n    role; the Alert carries its own permissions map (edit, share, list_tasks, list_logs); the Account\n    carries a permissions map and a team-member kind of admin, user or restricted. Some actions are\n    marked admin-only in the reference (setting a mention favorite or trashed, deleting another\n    account's share). None of that is exposed to the OAuth layer, so a client cannot request reduced\n    access —\
  \ it is all-or-nothing at the token, then filtered per resource at the server.\n  vocabulary_source: GET /app/data — alert_share_roles\n  cross_reference: data-model/mention-data-model.yml\nagent_implications:\n  - >-\n    An agent given a Mention token has full read AND write authority over the authorizing account:\n    it can delete accounts, delete shares (which destroys alerts), and create or modify anything.\n    There is no least-privilege token to issue instead.\n  - >-\n    Constrain at the agent layer rather than the token layer. See\n    agentic-access/mention-agentic-access.yml for the per-operation execution contracts.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/scopes/mention-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Alerts
- Brand Monitoring
- Media Monitoring
- Social Listening
- Social-Media
- Sentiment Analysis
- Reputation Management
- Influencer Marketing
- Competitive Intelligence
- Streaming
- Marketing
token_urls:
- https://web.mention.net/oauth/v2/token
---
