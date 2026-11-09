---
authorization_urls: []
description: 'The OAuth authorization-server metadata at api.find-ref.com declares exactly two

  scopes. The /connect/ documentation describes the allowed-range scope as read-only

  (evidence search, original-text lookup, citation cross-check) and the whole

  connector as free of charge from the user''s balance.

  '
docs: https://find-ref.com/connect/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Find Ref Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'find-ref publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the find-ref API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: find-ref
provider_slug: find-ref-com
schemes: []
scope_count: 2
scope_names:
- findref.read
- offline_access
scopes:
- description: Read-only access to find-ref's reference-search surface — evidence search, original-text lookup and citation cross-check against Korean statutes, enforcement decrees, accounting standards, court judgments and tribunal rulings.
  flows: []
  scope: findref.read
- description: Issue a refresh_token so the connector can refresh an access_token without re-prompting the user.
  flows: []
  scope: offline_access
slug: find-ref-com-scopes
source_filename: find-ref-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://api.find-ref.com/.well-known/oauth-authorization-server\ndocs: https://find-ref.com/connect/\nname: find-ref OAuth scopes\ndescription: |\n  The OAuth authorization-server metadata at api.find-ref.com declares exactly two\n  scopes. The /connect/ documentation describes the allowed-range scope as read-only\n  (evidence search, original-text lookup, citation cross-check) and the whole\n  connector as free of charge from the user's balance.\nscopes:\n  - name: findref.read\n    description: Read-only access to find-ref's reference-search surface — evidence search, original-text lookup and citation cross-check against Korean statutes, enforcement decrees, accounting standards, court judgments and tribunal rulings.\n  - name: offline_access\n    description: Issue a refresh_token so the connector can refresh an access_token without re-prompting the user.\nevidence:\n  - url: https://api.find-ref.com/.well-known/oauth-authorization-server\n\
  \    quote: '\"scopes_supported\":[\"findref.read\",\"offline_access\"]'\n    status: 200\n    fetched: '2026-11-07'\n"
source_yaml_url: https://artifacts.apis.io/find-ref-com/scopes/find-ref-com-scopes.yml
summary_line: 2 scopes
tags:
- Accounting
- Tax
- Legal Research
- Labor Law
- AI Assistant
- MCP
- Korea
- Reference Search
token_bound: false
token_urls: []
---
