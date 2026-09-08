---
authorization_urls: []
description: 'AnnounceKit runs a two-scope authorization model. It is unusually legible for its size: the scope list is machine-discoverable from the authorization server metadata, and the vendor publishes exactly which tools each scope unlocks.'
docs: https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Announcekit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AnnounceKit uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AnnounceKit
provider_slug: announcekit
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: announcekit-scopes
source_filename: announcekit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  scopes_supported read from the live RFC 8414 document at\n  https://announcekit.app/.well-known/oauth-authorization-server (HTTP 200,\n  fetched 2026-09-02), with descriptions taken verbatim from\n  https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit\n  and the announcekit-mcp 0.1.0 README.\ndocs: https://help.announcekit.app/en/articles/15827230-mcp-server-connect-your-ai-assistant-to-announcekit\nprovider: AnnounceKit\nproviderId: announcekit\ndescription: >-\n  AnnounceKit runs a two-scope authorization model. It is unusually legible for\n  its size: the scope list is machine-discoverable from the authorization server\n  metadata, and the vendor publishes exactly which tools each scope unlocks.\nissuer: https://announcekit.app\nauthorization_endpoint: https://announcekit.app/oauth/authorize\ntoken_endpoint: https://announcekit.app/oauth/token\nregistration_endpoint: https://announcekit.app/oauth/register\n\
  code_challenge_methods_supported: [S256]\nscope_count: 2\nscopes:\n- name: read\n  description: >-\n    Queries only. View posts, feedback, stats and roadmap. Exposes the 15 read\n    tools on the MCP server.\n  grants:\n  - MCP tools list_projects, list_labels, list_posts, get_post, list_post_templates,\n    get_post_stats, get_post_status_summary, list_feedback, list_activities, get_nps,\n    list_segments, list_external_users, list_feeds, list_feature_requests, list_roadmap\n- name: write\n  description: >-\n    Read, plus create and update content. No deletes. Exposes all 29 MCP tools.\n  grants:\n  - Everything in read\n  - MCP tools save_label, create_post, update_post, publish_post, schedule_post,\n    update_post_locale, save_post_template, generate_post_draft, improve_text,\n    create_feature_request, comment_feature_request, reply_feature_request,\n    create_roadmap_item, create_roadmap_status\nconstraints:\n- >-\n  Scope is not the only boundary. A token also inherits the\
  \ project access and\n  the ProjectRole (owner, manager, editor, viewer) of the member who created it,\n  and stops working on a project that member loses access to. The effective\n  permission is the intersection of scope and role.\n- >-\n  No scope grants deletion, billing or account administration on any surface -\n  those are not represented in the scope model at all.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/announcekit/refs/heads/main/scopes/announcekit-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Changelog
- Feature Requests
- NPS
- Notification
- Product Communication
- Roadmaps
- Software-as-a-Service
- Widgets
token_urls: []
---
