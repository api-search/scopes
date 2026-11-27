---
api_specs:
- filename: convertlyft-com-tools-api-openapi.yml
  format: yaml
  label: Convertlyft Tools API
  slug: convertlyft-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertlyft-com/openapi/convertlyft-com-tools-api-openapi.yml
authorization_urls: []
description: ''
docs: https://convertlyft.com/api/public/llms
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Convertlyft Scopes
name_suffix: OAuth Scopes
note: 'Scopes attach to cvl_pat_ personal access tokens and OAuth sign-ins; the OpenAPI declares only http bearer. Docs: holding some but not every listed scope is a 403; a connected app gets reads, plus crawl:run and seo:write only if the person ticks them, never memory:write or changes:write.'
overview: 'Convertlyft publishes 18 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Convertlyft API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Convertlyft
provider_slug: convertlyft-com
schemes: []
scope_count: 18
scope_names:
- workspaces:read
- reports:read
- sessions:read
- replays:read
- issues:read
- board:read
- changes:read
- changes:write
- proposals:read
- proposals:write
- operator:run
- memory:read
- memory:write
- issues:write
- crawl:run
- seo:write
- pages:write
- board:write
scopes:
- description: ''
  flows: []
  scope: workspaces:read
- description: ''
  flows: []
  scope: reports:read
- description: ''
  flows: []
  scope: sessions:read
- description: ''
  flows: []
  scope: replays:read
- description: ''
  flows: []
  scope: issues:read
- description: ''
  flows: []
  scope: board:read
- description: ''
  flows: []
  scope: changes:read
- description: ''
  flows: []
  scope: changes:write
- description: ''
  flows: []
  scope: proposals:read
- description: ''
  flows: []
  scope: proposals:write
- description: ''
  flows: []
  scope: operator:run
- description: ''
  flows: []
  scope: memory:read
- description: ''
  flows: []
  scope: memory:write
- description: ''
  flows: []
  scope: issues:write
- description: ''
  flows: []
  scope: crawl:run
- description: ''
  flows: []
  scope: seo:write
- description: ''
  flows: []
  scope: pages:write
- description: ''
  flows: []
  scope: board:write
slug: convertlyft-com-scopes
source_filename: convertlyft-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convertlyft.com/.well-known/convertlyft-capabilities.json\ndocs: https://convertlyft.com/api/public/llms\nnote: 'Scopes attach to cvl_pat_ personal access tokens and OAuth sign-ins; the OpenAPI declares only http bearer. Docs: holding some but not every listed scope is a 403; a connected app gets reads, plus\n  crawl:run and seo:write only if the person ticks them, never memory:write or changes:write.'\nscopes:\n- name: workspaces:read\n  access: read\n  used_by:\n  - cvl_connections_list\n  - cvl_install_verify\n  - cvl_workspaces_list\n- name: reports:read\n  access: read\n  used_by:\n  - cvl_attribution\n  - cvl_conversion_paths\n  - cvl_crawl_page\n  - cvl_crawl_status\n  - cvl_event_meanings\n  - cvl_explain\n  - cvl_forms\n  - cvl_funnel_report\n  - cvl_funnels_list\n  - cvl_kpi\n  - cvl_page_content\n  - cvl_page_type_rules\n  - cvl_page_types\n  - cvl_paths\n  - cvl_seo_agency_matrix\n  - cvl_seo_ai\n  - cvl_seo_audit\n\
  \  - cvl_seo_backlinks\n  - cvl_seo_brief\n  - cvl_seo_competitors\n  - cvl_seo_draft_status\n  - cvl_seo_drafts\n  - cvl_seo_flow\n  - cvl_seo_keyword\n  - cvl_seo_keywords\n  - cvl_seo_opportunities\n  - cvl_seo_overview\n  - cvl_seo_rank\n  - cvl_seo_search_console\n  - cvl_seo_server_logs\n  - cvl_seo_sitemaps\n  - cvl_site_pages\n  - cvl_usage\n- name: sessions:read\n  access: read\n  used_by:\n  - cvl_attribution\n  - cvl_behavior_report\n  - cvl_checkout_health\n  - cvl_checkout_values\n  - cvl_conversion_paths\n  - cvl_dead_clicks\n  - cvl_explain\n  - cvl_form_friction\n  - cvl_heatmap\n  - cvl_issue_detail\n  - cvl_kpi\n  - cvl_live_feed\n  - cvl_page_attention\n  - cvl_page_baselines\n  - cvl_page_conversions\n  - cvl_page_speed\n  - cvl_rage_clicks\n  - cvl_recommendations\n  - cvl_replay_moment\n  - cvl_sessions_search\n  - cvl_sessions_summary\n  - cvl_site_search\n  - cvl_traffic_breakdown\n  - cvl_watch\n- name: replays:read\n  access: read\n  used_by:\n  - cvl_replay_moment\n\
  \  - cvl_replays_list\n- name: issues:read\n  access: read\n  used_by:\n  - cvl_error_brief\n  - cvl_issue_detail\n  - cvl_issues_list\n- name: board:read\n  access: read\n  used_by:\n  - cvl_board_list\n  - cvl_todo_detail\n  - cvl_todos_list\n- name: changes:read\n  access: read\n  used_by:\n  - cvl_change_preview\n- name: changes:write\n  access: write\n  used_by:\n  - cvl_change_apply\n  - cvl_change_undo\n- name: proposals:read\n  access: read\n  used_by:\n  - cvl_proposals_list\n- name: proposals:write\n  access: write\n  used_by:\n  - cvl_propose\n- name: operator:run\n  access: write\n  used_by:\n  - POST /api/operator/run\n  - cvl_operator_run\n- name: memory:read\n  access: read\n  used_by:\n  - cvl_recall\n- name: memory:write\n  access: write\n  used_by:\n  - POST /api/memory\n  - cvl_remember\n- name: issues:write\n  access: write\n  used_by:\n  - cvl_error_fix_shipped\n- name: crawl:run\n  access: write\n  used_by:\n  - POST /api/crawl\n  - POST /api/crawl/[id]/webhook-secret\n\
  \  - cvl_crawl_start\n  - cvl_run_crawl\n- name: seo:write\n  access: write\n  used_by:\n  - POST /api/tools/[name]\n  - cvl_seo_add_keywords\n  - cvl_seo_add_market\n  - cvl_seo_ai_mentions\n  - cvl_seo_backlink_profile\n  - cvl_seo_brief_keywords\n  - cvl_seo_brief_published\n  - cvl_seo_check_now\n  - cvl_seo_competitor_gap\n  - cvl_seo_domain_overview\n  - cvl_seo_draft\n  - cvl_seo_draft_publish\n  - cvl_seo_issue_not_a_problem\n  - cvl_seo_issue_on_purpose\n  - cvl_seo_keyword_ideas\n  - cvl_seo_keyword_metrics\n  - cvl_seo_link_gap\n  - cvl_seo_make_brief\n  - cvl_seo_map_keyword_page\n  - cvl_seo_opportunity_set\n  - cvl_seo_opportunity_track\n  - cvl_seo_ranked_keywords\n  - cvl_seo_referring_domains\n  - cvl_seo_run_flow\n  - cvl_seo_serp\n  - cvl_seo_set_competitor_state\n  - cvl_seo_set_keyword_money\n  - cvl_seo_submit_sitemap\n  - cvl_seo_track_keywords\n  - cvl_seo_untrack_keywords\n  - cvl_seo_write_fix\n  - cvl_set_capture\n  - cvl_set_recording_paths\n- name: pages:write\n\
  \  access: write\n  used_by:\n  - cvl_remove_page_type_rule\n  - cvl_set_event_meaning\n  - cvl_set_form_purpose\n  - cvl_set_page_type\n  - cvl_set_site_type\n- name: board:write\n  access: write\n  used_by:\n  - POST /api/tools/[name]\n  - cvl_todo_add\n  - cvl_todo_mark\n"
source_yaml_url: https://artifacts.apis.io/convertlyft-com/scopes/convertlyft-com-scopes.yml
summary_line: 18 scopes
tags:
- Company
- Web Analytics
- Conversion Rate Optimization
- Session Replay
- Heatmaps
- SEO
- Error Tracking
- MCP
token_bound: false
token_urls: []
---
