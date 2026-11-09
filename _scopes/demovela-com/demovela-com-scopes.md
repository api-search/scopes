---
authorization_urls: []
description: ''
docs: https://github.com/demovela/mcp-server#permissions-and-account-access
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Demovela Com Scopes
name_suffix: OAuth Scopes
note: 'Scope strings are published verbatim for the MCP server ("Requested scopes: `profile:read videos:read drafts:write`"). The n8n/REST page describes the same permissions in prose ("read your profile, read videos and drafts, save drafts") without naming scope strings; REST tokens use a separate OAuth audience (https://demovela.com/v1).'
overview: 'Demovela publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Demovela API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demovela
provider_slug: demovela-com
schemes: []
scope_count: 3
scope_names:
- profile:read
- videos:read
- drafts:write
scopes:
- description: Read the signed-in account profile (get_profile / GET /v1/account).
  flows: []
  scope: profile:read
- description: Read owned videos and drafts and their status (list_videos, get_video, get_video_status).
  flows: []
  scope: videos:read
- description: Save a title, brief and template as a draft conversation (create_video_draft / POST /v1/video-drafts).
  flows: []
  scope: drafts:write
slug: demovela-com-scopes
source_filename: demovela-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Demovela OAuth scopes\ngenerated: '2026-11-05'\nmethod: searched\nsource: https://github.com/demovela/mcp-server\ndocs: https://github.com/demovela/mcp-server#permissions-and-account-access\nscopes:\n- name: profile:read\n  description: Read the signed-in account profile (get_profile / GET /v1/account).\n- name: videos:read\n  description: Read owned videos and drafts and their status (list_videos, get_video, get_video_status).\n- name: drafts:write\n  description: Save a title, brief and template as a draft conversation (create_video_draft / POST /v1/video-drafts).\nnote: 'Scope strings are published verbatim for the MCP server (\"Requested scopes: `profile:read videos:read drafts:write`\"). The n8n/REST page describes the same permissions in prose (\"read your profile, read videos and drafts, save drafts\") without naming scope strings; REST tokens use a separate OAuth audience (https://demovela.com/v1).'\n"
source_yaml_url: https://artifacts.apis.io/demovela-com/scopes/demovela-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- AI Video
- Product Demos
- Marketing Video
- Video Generation
- MCP
- n8n
- Software-as-a-Service
token_bound: false
token_urls: []
---
