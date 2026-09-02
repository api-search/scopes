---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Beaconsai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beacons.ai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beacons.ai
provider_slug: beaconsai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: beaconsai-scopes
source_filename: beaconsai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://beacons.ai/.well-known/oauth-authorization-server + https://beacons.ai/.well-known/oauth-protected-resource\ndocs: null\ndocs_note: >-\n  Beacons publishes no scopes/permissions reference page. Both discovery documents\n  independently advertise the same single scope, so the list below is complete as\n  published — but the meaning of the scope is undocumented and the description is\n  therefore limited to what the name and the protected resource state.\nissuer: https://beacons.ai\nresource: https://beacons.ai/api/v001/creator/mcp\nscope_count: 1\nscopes:\n- name: mcp:read\n  resource: https://beacons.ai/api/v001/creator/mcp\n  access: read\n  description: >-\n    Read access to the Beacons Creator MCP resource. Advertised by both\n    scopes_supported arrays; no scope description is published by the provider.\n  source: /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource\nobservations:\n- No\
  \ write scope is advertised, so the published agent surface is read-only.\n- Scope naming follows the MCP convention (`mcp:<action>`) rather than a\n  resource-per-scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconsai/refs/heads/main/scopes/beaconsai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Creator Economy
- Link in Bio
- Creator Website Builder
- Creator Storefront
- Media Kit
- Email Marketing
- Affiliate Marketing
- Creator Monetization
- Influencer Software
- MCP
- agent-native
token_urls: []
---
