---
authorization_urls: []
description: ''
docs: https://stellary.co/docs/api/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Stellary Scopes
name_suffix: OAuth Scopes
note: 'Stellary publishes no OpenAPI, so nothing here is derived from a spec. The OAuth set is read verbatim from live RFC 8414/RFC 9728 metadata; the two additional account/notification scopes come from the "Available scopes" list on the API tokens section of the REST reference. The two lists differ on purpose: the OAuth authorization server advertises the five scopes an MCP client can request, while a personal access token can carry seven. That gap is a real finding, not an omission -- an agent connecting over OAuth cannot obtain notifications:read, account:read or account:write, and the MCP 401 challenge names only the four project/pilotage scopes.'
overview: 'Stellary uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stellary
provider_slug: stellary
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: stellary-scopes
source_filename: stellary-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://stellary.co/docs/api/#api-tokens\ndocs: https://stellary.co/docs/api/\nprobed:\n- url: https://api.stellary.co/.well-known/oauth-authorization-server\n  status: 200\n  field: scopes_supported\n- url: https://api.stellary.co/.well-known/oauth-protected-resource/mcp\n  status: 200\n  field: scopes_supported\nnote: >-\n  Stellary publishes no OpenAPI, so nothing here is derived from a spec. The OAuth set is read\n  verbatim from live RFC 8414/RFC 9728 metadata; the two additional account/notification scopes\n  come from the \"Available scopes\" list on the API tokens section of the REST reference. The two\n  lists differ on purpose: the OAuth authorization server advertises the five scopes an MCP client\n  can request, while a personal access token can carry seven. That gap is a real finding, not an\n  omission -- an agent connecting over OAuth cannot obtain notifications:read, account:read or\n  account:write, and the\
  \ MCP 401 challenge names only the four project/pilotage scopes.\nauthorization_server: https://api.stellary.co/\nprotected_resource: https://api.stellary.co/mcp\nscopes:\n- name: projects:read\n  description: Read projects, boards, columns, cards, comments and delivery context.\n  oauth: true\n  personal_access_token: true\n  challenge_advertised: true\n- name: projects:write\n  description: Create and modify projects, cards, comments, assignments and card movement.\n  oauth: true\n  personal_access_token: true\n  challenge_advertised: true\n- name: pilotage:read\n  description: Read cockpit/pilotage state, dashboards, missions, priorities and pending proposals.\n  oauth: true\n  personal_access_token: true\n  challenge_advertised: true\n- name: pilotage:write\n  description: Create and act on pilotage actions, decisions and proposals.\n  oauth: true\n  personal_access_token: true\n  challenge_advertised: true\n- name: offline_access\n  description: Issue a rotating refresh token so the\
  \ client can renew the one-hour access token.\n  oauth: true\n  personal_access_token: false\n  challenge_advertised: false\n- name: notifications:read\n  description: Read account notifications.\n  oauth: false\n  personal_access_token: true\n  challenge_advertised: false\n- name: account:read\n  description: Read account profile data.\n  oauth: false\n  personal_access_token: true\n  challenge_advertised: false\n- name: account:write\n  description: Modify account profile data.\n  oauth: false\n  personal_access_token: true\n  challenge_advertised: false\nguidance:\n  provider_recommendation: >-\n    Stellary's own SKILL.md tells an agent to start with projects:read and pilotage:read and to add\n    write scopes only when needed.\n  enforcement: >-\n    Scope is not the only gate. Every call is rechecked against the selected identity's status,\n    project access, role, tool policy, autonomy mode and mission snapshot.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellary/refs/heads/main/scopes/stellary-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- project-management
- productivity
- AI-agents
- agent-orchestration
- MCP
- remote-mcp
- developer-tools
- SaaS
- collaboration
token_urls: []
---
