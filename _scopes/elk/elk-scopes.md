---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Elk Scopes
name_suffix: OAuth Scopes
note: 'THESE ARE MASTODON''S SCOPES, NOT ELK''S. Elk does not define a permission vocabulary; it requests a fixed, non-configurable set of top-level Mastodon scopes on every sign-in and never asks for less. That is a real finding about Elk''s consent posture: a user signing into Elk cannot grant read-only access, because the client hard-codes write, follow and push alongside read. There is no incremental or per-feature consent.'
overview: 'Elk uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elk
provider_slug: elk
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: elk-scopes
source_filename: elk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: derived\nsource: >-\n  Scope string read verbatim from Elk's published source —\n  https://github.com/elk-zone/elk/blob/main/server/api/[server]/login.ts (scope: 'read\n  write follow push') and the identical scope on the token exchange in\n  server/api/[server]/oauth/[origin].ts. Scope semantics from the Mastodon OAuth scopes\n  reference, https://docs.joinmastodon.org/api/oauth-scopes/ .\n  derive-oauth-scopes.py found 0 oauth2 schemes because Elk publishes no OpenAPI.\nprovider: Elk\nproviderId: elk\ndocs: null\nauthorizationUrl: https://{server}/oauth/authorize\ntokenUrl: https://{server}/oauth/token\nnote: >-\n  THESE ARE MASTODON'S SCOPES, NOT ELK'S. Elk does not define a permission vocabulary;\n  it requests a fixed, non-configurable set of top-level Mastodon scopes on every sign-in\n  and never asks for less. That is a real finding about Elk's consent posture: a user\n  signing into Elk cannot grant read-only access, because the client\
  \ hard-codes write,\n  follow and push alongside read. There is no incremental or per-feature consent.\nrequested_scopes:\n  - name: read\n    granted: always\n    description: Read all account data — timelines, statuses, notifications, lists, bookmarks, filters, search.\n  - name: write\n    granted: always\n    description: Create, edit and delete statuses and media; update account settings, lists, filters and bookmarks.\n  - name: follow\n    granted: always\n    description: Manage relationships — follow, unfollow, block, mute, and domain blocks.\n  - name: push\n    granted: always\n    description: Subscribe to and receive Web Push notifications for the account.\ngranularity:\n  incremental_consent: false\n  per_feature_scopes: false\n  read_only_option: false\n  evidence: >-\n    The scope string is a hard-coded literal in both the authorize-URL builder and the\n    token exchange. No code path narrows it and no setting exposes it.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elk/refs/heads/main/scopes/elk-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fediverse
- Mastodon
- Open-Source
- Social Networking
- Social-Media
- Web Client
- Progressive-Web-App
- Authentication
token_urls: []
---
