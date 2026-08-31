---
api_specs:
- filename: zype-platform.json
  format: json
  label: Zype Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-platform.json
- filename: zype-playout-scheduler.json
  format: json
  label: Zype Playout Scheduler API
  slug: playout-scheduler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-playout-scheduler.json
- filename: zype-monetization.json
  format: json
  label: Zype Monetization API
  slug: monetization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-monetization.json
- filename: zype-consumers.json
  format: json
  label: Zype Consumers API
  slug: consumers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-consumers.json
- filename: zype-live-3.json
  format: json
  label: Zype Live API (V3)
  slug: live-3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-live-3.json
- filename: zype-zobjects.json
  format: json
  label: Zype Zobjects API
  slug: zobjects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-zobjects.json
- filename: zype-analytics-v3.json
  format: json
  label: Zype Analytics API (V3)
  slug: analytics-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics-v3.json
- filename: zype-analytics.json
  format: json
  label: Zype Analytics API (V2)
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-analytics.json
- filename: zype-content-regions.json
  format: json
  label: Zype Custom Regions API
  slug: content-regions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-regions.json
- filename: zype-content-rule-groups.json
  format: json
  label: Zype Content Rule Groups API
  slug: content-rule-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rule-groups.json
- filename: zype-content-rules.json
  format: json
  label: Zype Content Rule Profiles API
  slug: content-rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-content-rules.json
- filename: zype-tve.json
  format: json
  label: Zype TVE API
  slug: tve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-tve.json
- filename: zype-login.json
  format: json
  label: Zype Consumer Authentication API
  slug: login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-login.json
- filename: zype-player.json
  format: json
  label: Zype Player API
  slug: player
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-player.json
- filename: zype-uploads.json
  format: json
  label: Zype Uploads API
  slug: uploads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/openapi/zype-uploads.json
authorization_urls: []
description: ''
docs: https://docs.zype.com/reference/oauth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zype Scopes
name_suffix: OAuth Scopes
note: The 148 scopes below are read verbatim from the scopes_supported array of Zype's RFC 8414 metadata document. The published OpenAPI files declare only apiKey and http bearer securitySchemes and carry no oauth2 flows object, so the scope list exists ONLY at the well-known endpoint — deriving it from the specs alone would have produced nothing. Descriptions are ours, expanded from the resource.action naming convention Zype uses; they are not provider prose.
overview: 'Zype uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zype
provider_slug: zype
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zype-scopes
source_filename: zype-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://api.zype.com/.well-known/oauth-authorization-server (HTTP 200, RFC 8414 Authorization Server Metadata)\ndocs: https://docs.zype.com/reference/oauth\nnote: The 148 scopes below are read verbatim from the scopes_supported array of Zype's RFC 8414 metadata document.\n  The published OpenAPI files declare only apiKey and http bearer securitySchemes and carry no oauth2 flows object,\n  so the scope list exists ONLY at the well-known endpoint — deriving it from the specs alone would have produced\n  nothing. Descriptions are ours, expanded from the resource.action naming convention Zype uses; they are not provider\n  prose.\nauthorization_endpoint: https://api.zype.com/oauth/authorize\ntoken_endpoint: https://api.zype.com/oauth/token\nintrospection_endpoint: https://api.zype.com/oauth/introspect\nrevocation_endpoint: https://api.zype.com/oauth/revoke\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- password\n\
  - refresh_token\ncode_challenge_methods_supported:\n- S256\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- none\nscope_count: 148\nsecond_issuer:\n  issuer: https://login.zype.com\n  note: login.zype.com serves an identical metadata document scoped to consumer (end-viewer) authentication; api.zype.com\n    serves the admin/platform side.\ngroups:\n- name: videos\n  scope_count: 5\n- name: video_sources\n  scope_count: 4\n- name: video_imports\n  scope_count: 3\n- name: segments\n  scope_count: 4\n- name: subtitles\n  scope_count: 4\n- name: transcriptions\n  scope_count: 3\n- name: subtitle_playlists\n  scope_count: 2\n- name: playlists\n  scope_count: 4\n- name: playlist_items\n  scope_count: 4\n- name: series\n  scope_count: 4\n- name: seasons\n  scope_count: 4\n- name: episodes\n  scope_count: 4\n- name: categories\n  scope_count: 4\n- name: zobjects\n  scope_count: 4\n- name: zobject_types\n  scope_count: 4\n- name: prompt_contexts\n  scope_count:\
  \ 4\n- name: content_rules\n  scope_count: 4\n- name: uploads\n  scope_count: 2\n- name: devices\n  scope_count: 2\n- name: live\n  scope_count: 9\n- name: playout\n  scope_count: 1\n- name: program_guides\n  scope_count: 4\n- name: live_events\n  scope_count: 4\n- name: apps\n  scope_count: 2\n- name: tve\n  scope_count: 1\n- name: consumers\n  scope_count: 8\n- name: plans\n  scope_count: 4\n- name: revenue_models\n  scope_count: 1\n- name: subscriptions\n  scope_count: 4\n- name: passes\n  scope_count: 4\n- name: ad_tags\n  scope_count: 4\n- name: ad_timings\n  scope_count: 4\n- name: redemption_codes\n  scope_count: 5\n- name: consumer_profile\n  scope_count: 1\n- name: consumer_entitlements\n  scope_count: 1\n- name: video_favorites\n  scope_count: 3\n- name: video_ratings\n  scope_count: 2\n- name: analytics\n  scope_count: 2\n- name: billing\n  scope_count: 4\n- name: account\n  scope_count: 1\n- name: transactions\n  scope_count: 4\n- name: usage\n  scope_count: 1\n- name: settings\n\
  \  scope_count: 2\n- name: analytics_bulk_export_jobs\n  scope_count: 2\n- name: user\n  scope_count: 1\nscopes:\n- name: videos.read\n  description: Read videos.\n- name: videos.create\n  description: Create videos.\n- name: videos.update\n  description: Update videos.\n- name: videos.delete\n  description: Delete videos.\n- name: videos.encode\n  description: Trigger encoding for videos.\n- name: video_sources.read\n  description: Read video sources.\n- name: video_sources.create\n  description: Create video sources.\n- name: video_sources.update\n  description: Update video sources.\n- name: video_sources.delete\n  description: Delete video sources.\n- name: video_imports.read\n  description: Read video imports.\n- name: video_imports.create\n  description: Create video imports.\n- name: video_imports.update\n  description: Update video imports.\n- name: segments.read\n  description: Read segments.\n- name: segments.create\n  description: Create segments.\n- name: segments.update\n\
  \  description: Update segments.\n- name: segments.delete\n  description: Delete segments.\n- name: subtitles.read\n  description: Read subtitles.\n- name: subtitles.create\n  description: Create subtitles.\n- name: subtitles.update\n  description: Update subtitles.\n- name: subtitles.delete\n  description: Delete subtitles.\n- name: transcriptions.read\n  description: Read transcriptions.\n- name: transcriptions.create\n  description: Create transcriptions.\n- name: transcriptions.update\n  description: Update transcriptions.\n- name: subtitle_playlists.create\n  description: Create subtitle playlists.\n- name: subtitle_playlists.delete\n  description: Delete subtitle playlists.\n- name: playlists.read\n  description: Read playlists.\n- name: playlists.create\n  description: Create playlists.\n- name: playlists.update\n  description: Update playlists.\n- name: playlists.delete\n  description: Delete playlists.\n- name: playlist_items.read\n  description: Read playlist items.\n- name:\
  \ playlist_items.create\n  description: Create playlist items.\n- name: playlist_items.update\n  description: Update playlist items.\n- name: playlist_items.delete\n  description: Delete playlist items.\n- name: series.read\n  description: Read series.\n- name: series.create\n  description: Create series.\n- name: series.update\n  description: Update series.\n- name: series.delete\n  description: Delete series.\n- name: seasons.read\n  description: Read seasons.\n- name: seasons.create\n  description: Create seasons.\n- name: seasons.update\n  description: Update seasons.\n- name: seasons.delete\n  description: Delete seasons.\n- name: episodes.read\n  description: Read episodes.\n- name: episodes.create\n  description: Create episodes.\n- name: episodes.update\n  description: Update episodes.\n- name: episodes.delete\n  description: Delete episodes.\n- name: categories.read\n  description: Read categories.\n- name: categories.create\n  description: Create categories.\n- name: categories.update\n\
  \  description: Update categories.\n- name: categories.delete\n  description: Delete categories.\n- name: zobjects.read\n  description: Read zobjects.\n- name: zobjects.create\n  description: Create zobjects.\n- name: zobjects.update\n  description: Update zobjects.\n- name: zobjects.delete\n  description: Delete zobjects.\n- name: zobject_types.read\n  description: Read zobject types.\n- name: zobject_types.create\n  description: Create zobject types.\n- name: zobject_types.update\n  description: Update zobject types.\n- name: zobject_types.delete\n  description: Delete zobject types.\n- name: prompt_contexts.read\n  description: Read prompt contexts.\n- name: prompt_contexts.create\n  description: Create prompt contexts.\n- name: prompt_contexts.update\n  description: Update prompt contexts.\n- name: prompt_contexts.delete\n  description: Delete prompt contexts.\n- name: content_rules.read\n  description: Read content rules.\n- name: content_rules.create\n  description: Create content\
  \ rules.\n- name: content_rules.update\n  description: Update content rules.\n- name: content_rules.delete\n  description: Delete content rules.\n- name: uploads.read\n  description: Read uploads.\n- name: uploads.create\n  description: Create uploads.\n- name: devices.read\n  description: Read devices.\n- name: devices.pair\n  description: Pair devices.\n- name: live.channels.read\n  description: Read live channels.\n- name: live.channels.create\n  description: Create live channels.\n- name: live.channels.update\n  description: Update live channels.\n- name: live.channels.delete\n  description: Delete live channels.\n- name: live.channels.start\n  description: Start live channels.\n- name: live.channels.stop\n  description: Stop live channels.\n- name: live.inputs.create\n  description: Create live inputs.\n- name: live.inputs.update\n  description: Update live inputs.\n- name: live.inputs.delete\n  description: Delete live inputs.\n- name: playout.read\n  description: Read playout.\n\
  - name: program_guides.read\n  description: Read program guides.\n- name: program_guides.create\n  description: Create program guides.\n- name: program_guides.update\n  description: Update program guides.\n- name: program_guides.delete\n  description: Delete program guides.\n- name: live_events.read\n  description: Read live events.\n- name: live_events.create\n  description: Create live events.\n- name: live_events.update\n  description: Update live events.\n- name: live_events.delete\n  description: Delete live events.\n- name: apps.read\n  description: Read apps.\n- name: apps.update\n  description: Update apps.\n- name: tve.authenticate\n  description: Authenticate against tve.\n- name: consumers.read\n  description: Read consumers.\n- name: consumers.create\n  description: Create consumers.\n- name: consumers.update\n  description: Update consumers.\n- name: consumers.delete\n  description: Delete consumers.\n- name: consumers.billing.read\n  description: Read consumers billing.\n\
  - name: consumers.billing.create\n  description: Create consumers billing.\n- name: consumers.billing.update\n  description: Update consumers billing.\n- name: consumers.billing.delete\n  description: Delete consumers billing.\n- name: plans.read\n  description: Read plans.\n- name: plans.create\n  description: Create plans.\n- name: plans.update\n  description: Update plans.\n- name: plans.delete\n  description: Delete plans.\n- name: revenue_models.read\n  description: Read revenue models.\n- name: subscriptions.read\n  description: Read subscriptions.\n- name: subscriptions.create\n  description: Create subscriptions.\n- name: subscriptions.update\n  description: Update subscriptions.\n- name: subscriptions.delete\n  description: Delete subscriptions.\n- name: passes.read\n  description: Read passes.\n- name: passes.create\n  description: Create passes.\n- name: passes.update\n  description: Update passes.\n- name: passes.delete\n  description: Delete passes.\n- name: ad_tags.read\n\
  \  description: Read ad tags.\n- name: ad_tags.create\n  description: Create ad tags.\n- name: ad_tags.update\n  description: Update ad tags.\n- name: ad_tags.delete\n  description: Delete ad tags.\n- name: ad_timings.read\n  description: Read ad timings.\n- name: ad_timings.create\n  description: Create ad timings.\n- name: ad_timings.update\n  description: Update ad timings.\n- name: ad_timings.delete\n  description: Delete ad timings.\n- name: redemption_codes.read\n  description: Read redemption codes.\n- name: redemption_codes.create\n  description: Create redemption codes.\n- name: redemption_codes.update\n  description: Update redemption codes.\n- name: redemption_codes.delete\n  description: Delete redemption codes.\n- name: consumer_profile.read\n  description: Read consumer profile.\n- name: consumer_entitlements.read\n  description: Read consumer entitlements.\n- name: video_favorites.read\n  description: Read video favorites.\n- name: video_favorites.create\n  description:\
  \ Create video favorites.\n- name: video_favorites.delete\n  description: Delete video favorites.\n- name: video_ratings.read\n  description: Read video ratings.\n- name: video_ratings.create\n  description: Create video ratings.\n- name: redemption_codes.redeem\n  description: Redeem redemption codes.\n- name: analytics.read\n  description: Read analytics.\n- name: analytics.export\n  description: Export analytics.\n- name: billing.read\n  description: Read billing.\n- name: billing.create\n  description: Create billing.\n- name: billing.update\n  description: Update billing.\n- name: billing.delete\n  description: Delete billing.\n- name: account.cancel\n  description: Cancel account.\n- name: transactions.read\n  description: Read transactions.\n- name: transactions.create\n  description: Create transactions.\n- name: transactions.update\n  description: Update transactions.\n- name: transactions.delete\n  description: Delete transactions.\n- name: usage.read\n  description: Read usage.\n\
  - name: settings.read\n  description: Read settings.\n- name: settings.update\n  description: Update settings.\n- name: analytics_bulk_export_jobs.read\n  description: Read analytics bulk export jobs.\n- name: analytics_bulk_export_jobs.create\n  description: Create analytics bulk export jobs.\n- name: user\n  description: Identify the authenticated user.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zype/refs/heads/main/scopes/zype-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Video
- Streaming
- OTT
- Video CMS
- FAST
- Linear TV
- Playout
- Monetization
- Live Streaming
- Analytics
- Media & Entertainment
- DRM
- Advertising
- Encoding
- EPG
token_urls: []
---
