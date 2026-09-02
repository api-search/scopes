---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Liftlab Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the scopes_supported array of LiftLab's RFC 8414 authorization-server metadata, corroborated by the identical scopes_supported in the RFC 9728 protected-resource document. LiftLab publishes no scopes or permissions reference page — there is no developer portal — so no description could be searched to enrich this. The single scope string is recorded as published; nothing is inferred about what it grants.
overview: 'LiftLab publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the LiftLab API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LiftLab
provider_slug: liftlab
schemes: []
scope_count: 1
scope_names:
- claudeai
scopes:
- description: The only scope advertised by the authorization server. Named for the Claude connector this MCP server is deployed for. LiftLab publishes no definition of what the scope grants, so none is asserted here.
  flows: []
  scope: claudeai
slug: liftlab-scopes
source_filename: liftlab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://connect.liftlab.com/.well-known/oauth-authorization-server\nnote: >-\n  Read verbatim from the scopes_supported array of LiftLab's RFC 8414\n  authorization-server metadata, corroborated by the identical scopes_supported\n  in the RFC 9728 protected-resource document. LiftLab publishes no scopes or\n  permissions reference page — there is no developer portal — so no description\n  could be searched to enrich this. The single scope string is recorded as\n  published; nothing is inferred about what it grants.\ndocs: null\ndocs_note: >-\n  No public scopes/permissions documentation exists. Probed liftlab.com\n  /developers/ (404), /api/ (404) and /docs (404) on 2026-08-13.\n\nauthorization_server: https://connect.liftlab.com\nprotected_resource: https://connect.liftlab.com/server/api/mcp\n\nscope_count: 1\nscopes:\n- scope: claudeai\n  description: >-\n    The only scope advertised by the authorization server. Named for\
  \ the Claude\n    connector this MCP server is deployed for. LiftLab publishes no definition of\n    what the scope grants, so none is asserted here.\n  source: scopes_supported\n  applies_to: https://connect.liftlab.com/server/api/mcp\n\nx-evidence:\n- url: https://connect.liftlab.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n  extract: '\"scopes_supported\": [\"claudeai\"]'\n- url: https://connect.liftlab.com/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n  extract: '\"scopes_supported\": [\"claudeai\"]'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liftlab/refs/heads/main/scopes/liftlab-scopes.yml
summary_line: 1 scope
tags:
- Company
- Enterprise
- Marketing
- Marketing Measurement
- Marketing Mix Modeling
- Incrementality
- Analytics
- MarTech
- Attribution
- Budget Optimization
- Data Science
- Software-as-a-Service
token_urls: []
---
