---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Peopleix Scopes
name_suffix: OAuth Scopes
note: 'peopleIX publishes no OpenAPI and no scopes/permissions reference page, so these scopes come straight from the anonymously-served OAuth metadata on the application host. Two facts matter here and are recorded rather than smoothed over: the AUTHORIZATION SERVER advertises only the two generic identity scopes below, and the PROTECTED RESOURCE (the MCP server) advertises an EMPTY scopes_supported array — meaning peopleIX exposes no per-tool or per-dataset scoping to a connecting agent. For a platform whose subject matter is employee-level HR data, the absence of a scope surface is the finding, not an omission in our capture.'
overview: 'Peopleix uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Peopleix
provider_slug: peopleix
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: peopleix-scopes
source_filename: peopleix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://app.peopleix.com/.well-known/oauth-authorization-server and https://app.peopleix.com/.well-known/oauth-protected-resource/mcp\nnote: >-\n  peopleIX publishes no OpenAPI and no scopes/permissions reference page, so these\n  scopes come straight from the anonymously-served OAuth metadata on the application\n  host. Two facts matter here and are recorded rather than smoothed over: the\n  AUTHORIZATION SERVER advertises only the two generic identity scopes below, and the\n  PROTECTED RESOURCE (the MCP server) advertises an EMPTY scopes_supported array —\n  meaning peopleIX exposes no per-tool or per-dataset scoping to a connecting agent.\n  For a platform whose subject matter is employee-level HR data, the absence of a\n  scope surface is the finding, not an omission in our capture.\ndocs: null\nauthorization_server: https://app.peopleix.com\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope requesting\
  \ an ID token identifying the authenticated\n    peopleIX user. Claims available: sub, iss, aud, exp, iat, email, name, org_id.\n  source: oauth-authorization-server scopes_supported\n- name: offline_access\n  description: >-\n    Requests a refresh token so an MCP client can maintain access without\n    re-prompting the user.\n  source: oauth-authorization-server scopes_supported\nresource_scopes:\n  resource: https://app.peopleix.com/mcp\n  scopes: []\n  note: >-\n    scopes_supported is an explicitly empty array in the RFC 9728 protected-resource\n    metadata. Access to the MCP tool surface therefore appears to be all-or-nothing\n    against the authenticated user's org membership (org_id claim), not scope-limited.\nscope_count: 2\nx-evidence:\n  fetched: '2026-08-14'\n  urls:\n  - url: https://app.peopleix.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://app.peopleix.com/.well-known/oauth-protected-resource/mcp\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleix/refs/heads/main/scopes/peopleix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- HR
- People Analytics
- People Intelligence
- Conversation Intelligence
- Human Resources
- Workforce Analytics
- AI
- MCP
- Germany
token_urls: []
---
