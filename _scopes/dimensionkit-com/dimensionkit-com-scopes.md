---
authorization_urls: []
description: ''
docs: https://dimensionkit.com/docs/mcp/tools/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dimensionkit Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DimensionKit publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DimensionKit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DimensionKit
provider_slug: dimensionkit-com
schemes: []
scope_count: 2
scope_names:
- scorecards:read
- scorecards:write
scopes:
- description: View your scorecards, their configuration, and submissions
  flows: []
  scope: scorecards:read
- description: Create, edit, and publish your scorecards
  flows: []
  scope: scorecards:write
slug: dimensionkit-com-scopes
source_filename: dimensionkit-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dimensionkit.com/docs/mcp/connecting/\ndocs: https://dimensionkit.com/docs/mcp/tools/\nname: DimensionKit OAuth scopes\nscopes:\n- name: scorecards:read\n  description: View your scorecards, their configuration, and submissions\n  tools: [scorecard_design_guide, list_scorecards, get_scorecard, check_scorecard, list_submissions, get_submission]\n- name: scorecards:write\n  description: Create, edit, and publish your scorecards\n  tools: [create_scorecard, update_scorecard_config, add_dimension, add_questions, add_question, set_dimension_tiers, update_dimension, update_question, remove_question, remove_dimension, publish_scorecard]\nnotes:\n- A connection granted only scorecards:read cannot call a writing tool; it gets an error naming the scope it is missing.\n- Scopes are fixed for the life of a connection; disconnect and reconnect to change them.\n- Scopes advertised in scopes_supported of https://app.dimensionkit.com/.well-known/oauth-protected-resource\
  \ (HTTP 200).\n"
source_yaml_url: https://artifacts.apis.io/dimensionkit-com/scopes/dimensionkit-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Assessment
- Scorecards
- Lead Generation
- MCP
- Artificial Intelligence
- Quizzes
token_bound: false
token_urls: []
---
