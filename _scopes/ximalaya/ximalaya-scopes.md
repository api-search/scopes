---
authorization_urls: []
description: ''
docs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=75
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ximalaya Scopes
name_suffix: OAuth Scopes
note: 'Derived by SEARCH, not by derive-oauth-scopes.py: Ximalaya publishes no OpenAPI, so there are no oauth2 securityScheme flows to read. The scope list below is quoted verbatim from the scope string returned in the documented /oauth2/v2/access_token response example.'
overview: 'Ximalaya uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ximalaya
provider_slug: ximalaya
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ximalaya-scopes
source_filename: ximalaya-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=5 (OAuth2 标准登录授权API)\ndocs: https://open.ximalaya.com/doc/detailApi?categoryId=9&articleId=75\nnote: >-\n  Derived by SEARCH, not by derive-oauth-scopes.py: Ximalaya publishes no OpenAPI, so\n  there are no oauth2 securityScheme flows to read. The scope list below is quoted\n  verbatim from the scope string returned in the documented /oauth2/v2/access_token\n  response example.\n\nauthorization_endpoint: https://api.ximalaya.com/oauth2/v2/authorize\ntoken_endpoint: https://api.ximalaya.com/oauth2/v2/access_token\nscope_delimiter: ','\nscope_count: 6\n\nscopes:\n- name: profile:read\n  description: Read the authorizing user's basic profile and persona data.\n  backing_operations:\n  - /profile/user_info\n  - /profile/persona\n- name: subscribe:read\n  description: Read the authorizing user's album subscriptions.\n  backing_operations:\n  - /v2/subscribe/get_albums_by_uid\n\
  \  - /v2/subscribe/is_subscribed\n- name: subscribe:write\n  description: Add or remove album subscriptions for the authorizing user.\n  backing_operations:\n  - /subscribe/add_or_delete\n  - /subscribe/batch_add\n- name: play_history:read\n  description: Read the authorizing user's cloud play history.\n  backing_operations:\n  - /play_history/get_by_uid\n- name: play_history:write\n  description: Upload or delete entries in the authorizing user's cloud play history.\n  backing_operations:\n  - /play_history/batch_upload\n  - /play_history/batch_delete\n- name: open_pay:read\n  description: Read the authorizing user's paid-content entitlements and purchase state.\n  backing_operations:\n  - /open_pay/get_bought\n  - /v2/open_pay/get_bought_albums\n  - /open_pay/album_bought_status\n  - /open_pay/track_bought_status\n\nerrors:\n- code: 202\n  string: ximalaya.oauth2.scope_grant_denied\n  meaning: Scope authorization denied because the requested scope is invalid or exceeds\n    what the\
  \ application was granted.\n\ngaps:\n- Ximalaya does not publish a standalone scopes/permissions reference page; the scope\n  set above is the one enumerated in the token-response example. Additional scopes may\n  exist for partners with broader commercial agreements and would not be visible here.\n- Scope-to-operation binding above is inferred from which documented endpoints require\n  the user-private-data common parameter set (access_token + pack_id); Ximalaya does not\n  publish a per-endpoint scope table.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ximalaya/refs/heads/main/scopes/ximalaya-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Audio
- Podcasts
- Audiobooks
- Media
- Content Distribution
- Streaming
- China
- Entertainment
token_urls: []
---
