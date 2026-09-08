---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Wellfound Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wellfound uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wellfound
provider_slug: wellfound
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wellfound-scopes
source_filename: wellfound-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://wellfound.com/.well-known/openid-configuration (200),\n  https://wellfound.com/.well-known/oauth-protected-resource (200),\n  https://reach.wellfound.com/.well-known/oauth-authorization-server (200),\n  https://reach.wellfound.com/.well-known/oauth-protected-resource (200)\ndocs: null\ndocs_note: >-\n  No scopes / permissions reference page exists on any Wellfound property. The scope\n  vocabulary below was read verbatim out of the scopes_supported arrays of the four\n  discovery documents; the descriptions are our plain reading of each scope name and are\n  marked as such. Wellfound publishes no prose definition of any of these scopes.\n\nauthorization_servers:\n- issuer: https://wellfound.com\n  scope_count: 9\n  protects: https://wellfound.com/api/mcp\n  scopes:\n  - name: message\n    description: legacy AngelList-era scope - no published definition\n    described_by_provider: false\n    used_by_live_resource:\
  \ false\n  - name: dealflow\n    description: legacy AngelList-era scope - no published definition\n    described_by_provider: false\n    used_by_live_resource: false\n  - name: comment\n    description: legacy AngelList-era scope - no published definition\n    described_by_provider: false\n    used_by_live_resource: false\n  - name: email\n    description: read the authenticated member's email address (our reading of the name)\n    described_by_provider: false\n    used_by_live_resource: false\n  - name: invest\n    description: legacy AngelList-era scope - no published definition\n    described_by_provider: false\n    used_by_live_resource: false\n  - name: accreditation\n    description: legacy AngelList-era scope - no published definition\n    described_by_provider: false\n    used_by_live_resource: false\n  - name: applications:read\n    description: read a recruiter's inbound job applications (our reading of the name)\n    described_by_provider: false\n    used_by_live_resource:\
  \ true\n  - name: applications:accept\n    description: accept an inbound application - a WRITE scope with an irreversible-looking\n      effect on a candidate\n    described_by_provider: false\n    used_by_live_resource: true\n  - name: applications:reject\n    description: reject an inbound application - a WRITE scope with an irreversible-looking\n      effect on a candidate\n    described_by_provider: false\n    used_by_live_resource: true\n- issuer: https://reach.wellfound.com\n  scope_count: 7\n  protects: https://reach.wellfound.com/mcp\n  scopes:\n  - name: projects:read\n    description: read sourcing projects\n    described_by_provider: false\n    write: false\n  - name: agents:read\n    description: read the AI sourcing agents configured on the account\n    described_by_provider: false\n    write: false\n  - name: agents:write\n    description: create or modify AI sourcing agents\n    described_by_provider: false\n    write: true\n  - name: candidates:read\n    description: read\
  \ candidates\n    described_by_provider: false\n    write: false\n  - name: candidates:write\n    description: create or modify candidates\n    described_by_provider: false\n    write: true\n  - name: company_lists:read\n    description: read company lists\n    described_by_provider: false\n    write: false\n  - name: company_lists:write\n    description: create or modify company lists\n    described_by_provider: false\n    write: true\n\nanalysis:\n  total_scopes: 16\n  granularity: >-\n    The Reach server is cleanly resource:action scoped (7 scopes over 4 resources, read and\n    write split on each). The wellfound.com server is not: six of its nine scopes are bare\n    verbs or nouns inherited from the AngelList era with no separator and no published\n    definition, and only the three colon-scoped applications:* entries belong to the live MCP\n    resource. An agent asking for consent on this server cannot tell a user what \"dealflow\"\n    or \"invest\" would let it do.\n  least_privilege_possible:\
  \ true\n  least_privilege_note: >-\n    Both servers do split read from write, so a read-only agent can be granted read-only\n    access. On the applications server the split is finer than usual - accept and reject are\n    separate scopes, so an agent can be permitted to accept but not reject, or the reverse.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellfound/refs/heads/main/scopes/wellfound-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Recruiting
- Hiring
- Talent
- Human Resources
- Applicant Tracking
- Job Board
- Startups
- MCP
- agent-native
- OAuth
- AI Sourcing
token_urls: []
---
