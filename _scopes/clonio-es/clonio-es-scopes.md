---
authorization_urls: []
description: ''
docs: https://clonio.es/ayuda/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clonio Scopes
name_suffix: OAuth Scopes
note: Scope names from scopes_supported in the protected-resource and authorization-server metadata (both HTTP 200). The docs page describes permissions in prose only and gives no per-scope reference; descriptions above paraphrase that prose, null where it says nothing.
overview: 'Clonio publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clonio API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clonio
provider_slug: clonio-es
schemes: []
scope_count: 7
scope_names:
- account:read
- posts:read
- posts:write
- posts:publish
- insights:read
- ai:generate
- images:generate
scopes:
- description: ''
  flows: []
  scope: account:read
- description: ''
  flows: []
  scope: posts:read
- description: ''
  flows: []
  scope: posts:write
- description: 'Sensitive: publish to LinkedIn; docs say publishing always goes through a preview with the exact text and a confirmation.'
  flows: []
  scope: posts:publish
- description: ''
  flows: []
  scope: insights:read
- description: ''
  flows: []
  scope: ai:generate
- description: 'Sensitive outside Claude: spends image credits.'
  flows: []
  scope: images:generate
slug: clonio-es-scopes
source_filename: clonio-es-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-04''

  method: probed

  source: https://clonio.es/.well-known/oauth-protected-resource

  docs: https://clonio.es/ayuda/mcp

  scopes:

  - {name: ''account:read'', description: null}

  - {name: ''posts:read'', description: null}

  - {name: ''posts:write'', description: null}

  - {name: ''posts:publish'', description: ''Sensitive: publish to LinkedIn; docs say publishing always goes through a preview with the exact text and a confirmation.''}

  - {name: ''insights:read'', description: null}

  - {name: ''ai:generate'', description: null}

  - {name: ''images:generate'', description: ''Sensitive outside Claude: spends image credits.''}

  note: Scope names from scopes_supported in the protected-resource and authorization-server metadata (both HTTP 200). The docs page describes permissions in prose only and gives no per-scope reference; descriptions above paraphrase that prose, null where it says nothing.

  '
source_yaml_url: https://artifacts.apis.io/clonio-es/scopes/clonio-es-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Artificial Intelligence
- LinkedIn
- Content Generation
- Social Media
- Marketing
- Scheduling
- MCP
token_bound: false
token_urls: []
---
