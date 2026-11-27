---
authorization_urls: []
description: Scopes advertised in scopes_supported by both the protected-resource metadata and the authorization-server metadata (https://coverthegaps.com/.well-known/oauth-authorization-server). The provider publishes no scope reference page; descriptions are not stated by the provider beyond the agents page line "Reading and changing are asked for separately."
docs: https://coverthegaps.com/agents/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CoverTheGaps Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoverTheGaps publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoverTheGaps API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoverTheGaps
provider_slug: coverthegaps-com
schemes:
- authorizationUrl: https://coverthegaps.com/o/authorize/
  name: CoverTheGaps MCP OAuth
  tokenUrl: https://coverthegaps.com/o/token/
  type: oauth2
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: ''
  flows: []
  scope: mcp:read
- description: ''
  flows: []
  scope: mcp:write
- description: ''
  flows: []
  scope: offline_access
slug: coverthegaps-com-scopes
source_filename: coverthegaps-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://coverthegaps.com/.well-known/oauth-protected-resource\ndocs: https://coverthegaps.com/agents/\ndescription: >-\n  Scopes advertised in scopes_supported by both the protected-resource metadata and the authorization-server\n  metadata (https://coverthegaps.com/.well-known/oauth-authorization-server). The provider publishes no scope\n  reference page; descriptions are not stated by the provider beyond the agents page line \"Reading and changing\n  are asked for separately.\"\nschemes:\n- name: CoverTheGaps MCP OAuth\n  type: oauth2\n  authorizationUrl: https://coverthegaps.com/o/authorize/\n  tokenUrl: https://coverthegaps.com/o/token/\nscopes:\n- scope: mcp:read\n  description: null\n  schemes: [CoverTheGaps MCP OAuth]\n- scope: mcp:write\n  description: null\n  schemes: [CoverTheGaps MCP OAuth]\n- scope: offline_access\n  description: null\n  note: Paired with the advertised refresh_token grant.\n  schemes: [CoverTheGaps\
  \ MCP OAuth]\n"
source_yaml_url: https://artifacts.apis.io/coverthegaps-com/scopes/coverthegaps-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Education
- Language Learning
- English Teaching
- Tutoring
- Homework
- MCP
- AI Assistant
token_bound: false
token_urls: []
---
