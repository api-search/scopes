---
authorization_urls: []
description: ''
docs: https://conferencegrid.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: ConferenceGrid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ConferenceGrid publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the ConferenceGrid API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ConferenceGrid
provider_slug: conferencegrid-com
schemes: []
scope_count: 1
scope_names:
- conferences:read
scopes:
- description: Read-only access to the ConferenceGrid conference catalogue through the MCP server (all nine tools are read-only).
  flows: []
  scope: conferences:read
slug: conferencegrid-com-scopes
source_filename: conferencegrid-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://conferencegrid.com/.well-known/oauth-authorization-server\ndocs: https://conferencegrid.com/mcp\nscopes:\n- name: conferences:read\n  description: Read-only access to the ConferenceGrid conference catalogue through the MCP server (all nine tools are read-only).\n  evidence: scopes_supported [\"conferences:read\"] in both /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource (HTTP 200).\n"
source_yaml_url: https://artifacts.apis.io/conferencegrid-com/scopes/conferencegrid-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- Conferences
- Event
- Trade Shows
- Sales Intelligence
- B2B
- Sponsorship
- MCP
token_bound: false
token_urls: []
---
