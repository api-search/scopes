---
authorization_urls: []
description: The complete scope set Solve Intelligence advertises for its MCP resource server, read verbatim from the scopes_supported array of its RFC 9728 protected-resource metadata and corroborated by the scope parameter in the WWW-Authenticate challenge returned on an unauthenticated call. Both scopes are required together by the challenge.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Solve Intelligence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Solve Intelligence uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Solve Intelligence
provider_slug: solve-intelligence
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: solve-intelligence-scopes
source_filename: solve-intelligence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://api.solveintelligence.com/.well-known/oauth-protected-resource\nname: Solve Intelligence OAuth scopes\ndescription: >-\n  The complete scope set Solve Intelligence advertises for its MCP resource server, read\n  verbatim from the scopes_supported array of its RFC 9728 protected-resource metadata and\n  corroborated by the scope parameter in the WWW-Authenticate challenge returned on an\n  unauthenticated call. Both scopes are required together by the challenge.\ndocs: null\ndocs_note: >-\n  The provider publishes no scopes/permissions reference page. These values come from the\n  machine-readable metadata document itself, which is the authoritative source.\nauthorization_server: https://api.solveintelligence.com/auth\nresource: https://api.solveintelligence.com/mcp/\n\nscopes:\n  - name: offline_access\n    description: >-\n      Standard OpenID Connect scope requesting a refresh token, so an MCP client can renew its\n\
  \      access token without sending the user back through a browser sign-in.\n    standard: true\n    specification: OpenID Connect Core 1.0\n  - name: mcp:ask_solve\n    description: >-\n      Grants access to the Solve MCP research surface - patent and non-patent literature search,\n      jurisdictional legal-text and case-law search, and SEP standard documentation search.\n    standard: false\n    note: >-\n      The scope name carries the server's tool name, ask_solve. The tool's input schema was not\n      observable anonymously.\n\nscope_count: 2\ngranularity: coarse\ngranularity_note: >-\n  One functional scope covers the entire research surface. There is no read/write split and no\n  per-capability scope, so an agent granted mcp:ask_solve receives every capability the server\n  exposes. This is typical for a single-tool MCP server and is recorded as an observation, not a\n  defect.\n\nevidence:\n  - url: https://api.solveintelligence.com/.well-known/oauth-protected-resource\n \
  \   status: 200\n  - url: https://api.solveintelligence.com/mcp/\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solve-intelligence/refs/heads/main/scopes/solve-intelligence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Legal
- Legal Tech
- Intellectual Property
- Patents
- Artificial Intelligence
- Document Generation
- Search
- MCP
- Agents
token_urls: []
---
