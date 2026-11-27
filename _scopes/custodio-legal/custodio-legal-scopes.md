---
authorization_urls: []
description: ''
docs: https://docs.custodio.legal/en/manual/24-conectar-custodio-a-tu-asistente/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Custodio Legal Scopes
name_suffix: OAuth Scopes
note: Scope names come verbatim from the protected-resource document's scopes_supported; descriptions paraphrase the permissions paragraph of the docs page, which does not name scopes one by one.
overview: 'Custodio Legal publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Custodio Legal API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Custodio Legal
provider_slug: custodio-legal
schemes: []
scope_count: 5
scope_names:
- matters:read
- intelligence:read
- knowledge:search
- drafts:prepare
- offline_access
scopes:
- description: Reading matters (docs - "Available permissions include reading matters and intelligence").
  flows: []
  scope: matters:read
- description: Reading intelligence (AI output over matters).
  flows: []
  scope: intelligence:read
- description: Searching retained knowledge.
  flows: []
  scope: knowledge:search
- description: Preparing drafts/actions for human approval inside Custodio; per docs preparing actions requires the Pro, Max or Teams plan.
  flows: []
  scope: drafts:prepare
- description: Keeping the connection active (refresh); docs - "Connection renewal grants no additional access."
  flows: []
  scope: offline_access
slug: custodio-legal-scopes
source_filename: custodio-legal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://custodio.legal/.well-known/oauth-protected-resource\ndocs: https://docs.custodio.legal/en/manual/24-conectar-custodio-a-tu-asistente/\nresource: https://custodio.legal/mcp\nscopes:\n- name: matters:read\n  description: Reading matters (docs - \"Available permissions include reading matters and intelligence\").\n- name: intelligence:read\n  description: Reading intelligence (AI output over matters).\n- name: knowledge:search\n  description: Searching retained knowledge.\n- name: drafts:prepare\n  description: Preparing drafts/actions for human approval inside Custodio; per docs preparing actions requires the Pro, Max or Teams plan.\n- name: offline_access\n  description: Keeping the connection active (refresh); docs - \"Connection renewal grants no additional access.\"\nnote: Scope names come verbatim from the protected-resource document's scopes_supported; descriptions paraphrase the permissions paragraph of the docs\
  \ page, which does not name scopes one by one.\n"
source_yaml_url: https://artifacts.apis.io/custodio-legal/scopes/custodio-legal-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Legal
- Legal Tech
- Practice Management
- Judicial Monitoring
- Artificial Intelligence
- MCP
- Latin America
- Colombia
token_bound: false
token_urls: []
---
