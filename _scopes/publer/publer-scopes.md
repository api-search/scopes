---
api_specs:
- filename: publer-accounts-api-openapi.yml
  format: yaml
  label: Publer Accounts API
  slug: publer-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-accounts-api-openapi.yml
- filename: publer-analytics-api-openapi.yml
  format: yaml
  label: Publer Analytics API
  slug: publer-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-analytics-api-openapi.yml
- filename: publer-competitors-api-openapi.yml
  format: yaml
  label: Publer Competitors API
  slug: publer-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-competitors-api-openapi.yml
- filename: publer-jobs-api-openapi.yml
  format: yaml
  label: Publer Jobs API
  slug: publer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-jobs-api-openapi.yml
- filename: publer-media-api-openapi.yml
  format: yaml
  label: Publer Media API
  slug: publer-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-media-api-openapi.yml
- filename: publer-posts-api-openapi.yml
  format: yaml
  label: Publer Posts API
  slug: publer-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-posts-api-openapi.yml
- filename: publer-users-api-openapi.yml
  format: yaml
  label: Publer Users API
  slug: publer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-users-api-openapi.yml
- filename: publer-workspaces-api-openapi.yml
  format: yaml
  label: Publer Workspaces API
  slug: publer-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-workspaces-api-openapi.yml
authorization_urls: []
description: ''
docs: https://publer.com/docs/getting-started/authentication.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Publer Scopes
name_suffix: OAuth Scopes
note: 'THESE ARE NOT OAUTH 2.0 SCOPES. Publer runs no OAuth 2.0 authorization server and issues no access tokens — there is no authorization endpoint, no token endpoint, and no /.well-known/oauth-authorization-server (probed 2026-08-13: publer.com returns the Framer SPA shell, app.publer.com returns 410). What Publer publishes is a real, user-selected PERMISSION SCOPE model bound to a long-lived API key: the user picks scopes when the key is created in Settings -> API & Webhooks, and the same scope set governs both REST and MCP access. Recorded here because it is the provider''s published permission reference.'
overview: 'Publer uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Publer
provider_slug: publer
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: publer-scopes
source_filename: publer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://publer.com/docs/getting-started/authentication.md\nsource: >-\n  https://publer.com/docs/getting-started/authentication.md (\"API Key Scopes\"\n  table), https://publer.com/docs/getting-started/quickstart.md,\n  https://publer.com/help/en/article/how-to-access-the-publer-api-1w08edo/ and\n  https://publer.com/help/en/article/how-to-set-up-and-use-publers-mcp-server-14orlq0/\nprovider: Publer\nproviderId: publer\n\nscheme: api-key-scopes\noauth2: false\nnote: >-\n  THESE ARE NOT OAUTH 2.0 SCOPES. Publer runs no OAuth 2.0 authorization server\n  and issues no access tokens — there is no authorization endpoint, no token\n  endpoint, and no /.well-known/oauth-authorization-server (probed 2026-08-13:\n  publer.com returns the Framer SPA shell, app.publer.com returns 410). What\n  Publer publishes is a real, user-selected PERMISSION SCOPE model bound to a\n  long-lived API key: the user picks scopes when the key is created\
  \ in Settings\n  -> API & Webhooks, and the same scope set governs both REST and MCP access.\n  Recorded here because it is the provider's published permission reference.\n\ngrant_flow: none\nconsent_ui: in-app key creation dialog\nscope_selection: per-key, chosen by the user at creation time\ndownscoping: >-\n  Publer recommends creating separate keys per use case (least privilege). A\n  key's scopes cannot be changed after creation — remove the key and create a\n  new one.\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_body: '{\"errors\": [\"...\"]}'\n  note: >-\n    403 also signals a missing Publer-Workspace-Id header and a missing plan\n    entitlement, so an insufficient-scope failure is not distinguishable by\n    status alone.\n\nscopes:\n- name: workspaces\n  description: Retrieve the user's workspaces.\n  required: true\n  required_note: Selected by default and mandatory on every key.\n  example_endpoints:\n  - GET /workspaces\n  operations:\n  - listWorkspaces\n\
  \  consequence: read\n- name: accounts\n  description: Retrieve the user's connected social accounts for the selected workspace.\n  required: true\n  required_note: Selected by default and mandatory on every key.\n  example_endpoints:\n  - GET /accounts\n  operations:\n  - listAccounts\n  consequence: read\n- name: posts\n  description: Manage the user's posts — list, schedule, publish, update and delete.\n  required: false\n  example_endpoints:\n  - GET /posts\n  - POST /posts/schedule\n  - POST /posts/schedule/publish\n  - PUT /posts/{id}\n  - DELETE /posts\n  - GET /job_status/{job_id}\n  operations:\n  - listPosts\n  - schedulePosts\n  - createPost\n  - updatePost\n  - deleteMultiplePosts\n  - getJobStatus\n  consequence: write\n  note: >-\n    A single scope covers both read and write on posts. There is no read-only\n    posts scope, so any integration that needs to LIST posts is also granted the\n    ability to PUBLISH and DELETE them. This is the sharpest least-privilege gap\n \
  \   in Publer's scope model.\n- name: media\n  description: Upload and list media assets in the workspace library.\n  required: false\n  example_endpoints:\n  - GET /media\n  - POST /media\n  - POST /media/from-url\n  operations:\n  - listMedia\n  - uploadAMediaFileDirectly\n  - uploadMediaFromURL\n  consequence: write\n- name: analytics\n  description: >-\n    Read analytics — charts, chart data, post insights, hashtag analysis, best\n    times to post, member activity and competitor analysis.\n  required: false\n  example_endpoints:\n  - GET /analytics/charts\n  - GET /analytics/chart_data\n  - GET /analytics/{account_id}/post_insights\n  - GET /analytics/{account_id}/best_times\n  - GET /analytics/{account_id}/hashtag_insights\n  - GET /analytics/members\n  - GET /competitors/{account_id}\n  operations:\n  - getAvailableAnalyticsCharts\n  - getAnalyticsChartData\n  - getPostInsights\n  - getBestTimesToPostForAccount\n  - getHashtagInsights\n  - getHashtagPerformingPosts\n  - getAnalyticsMembersData\n\
  \  - listCompetitors\n  - getCompetitorsAnalytics\n  consequence: read\n  note: >-\n    Named in the help center and MCP setup articles (\"select any additional\n    scopes ... such as Posts, Media, or Analytics\") but MISSING from the scope\n    table in the developer docs, which lists only workspaces, accounts, posts\n    and media. The analytics endpoints additionally return 403 \"requires\n    analytics access or paying subscription\", so scope alone is not sufficient.\n\ngaps:\n- The docs scope table omits `analytics`, which the help center documents.\n- No read-only variant of `posts` or `media`; read and write share one scope.\n- No scope is declared in the OpenAPI security requirements — the spec declares\n  only the apiKey scheme, so scope requirements are not machine-readable\n  per-operation. The operation mappings above are ours, derived from the docs.\n\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/scopes/publer-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Social-Media
- Scheduling
- Publishing
- Content Management
- Marketing
- Social Media Management
- Analytics
- Agents
- MCP
- Automation
token_urls: []
---
