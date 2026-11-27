---
authorization_urls: []
description: ''
docs: https://compslate.com/docs/connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CompSlate Scopes
name_suffix: OAuth Scopes
note: The protected-resource and authorization-server metadata both list a single scope, "comp". The docs publish no scope reference; what a token can do is decided by the connecting person's workspace role (admin, manager, member), per https://compslate.com/docs/access.
overview: 'CompSlate publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CompSlate API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CompSlate
provider_slug: compslate-com
schemes: []
scope_count: 1
scope_names:
- comp
scopes:
- description: Single scope for the CompSlate MCP server; no description is published. Effective permissions follow the signed-in person's role.
  flows: []
  scope: comp
slug: compslate-com-scopes
source_filename: compslate-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://compslate.com/.well-known/oauth-protected-resource\ndocs: https://compslate.com/docs/connect\nnote: The protected-resource and authorization-server metadata both list a single scope, \"comp\". The docs publish no scope reference; what a token can do is decided by the connecting person's workspace role (admin, manager, member), per https://compslate.com/docs/access.\nscopes:\n- name: comp\n  description: Single scope for the CompSlate MCP server; no description is published. Effective permissions follow the signed-in person's role.\n  source: https://compslate.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/compslate-com/scopes/compslate-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- Sales Compensation
- Sales Commissions
- Revenue Operations
- MCP
- AI Assistant
- Software-as-a-Service
token_bound: false
token_urls: []
---
