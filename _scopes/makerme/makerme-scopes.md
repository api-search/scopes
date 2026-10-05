---
authorization_urls: []
description: ''
docs: https://docs.maker.co/features/use-maker-from-your-ai-assistant
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Makerme Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Maker.me publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Maker.me API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Maker.me
provider_slug: makerme
schemes: []
scope_count: 2
scope_names:
- maker:read
- maker:publish
scopes:
- description: Read access to the connected Maker account — list and open projects, read project insights, and screenshot previews.
  flows: []
  scope: maker:read
- description: Publish and mutation access — edit copy, swap images, generate new sections, create variants, set up A/B tests, and push changes live.
  flows: []
  scope: maker:publish
slug: makerme-scopes
source_filename: makerme-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  ai.maker.co/.well-known/oauth-authorization-server and\n  oauth-protected-resource (scopes_supported), 2026-07-20\noauth:\n  issuer: https://ai.maker.co\n  resource: https://ai.maker.co/mcp\nscopes:\n- name: maker:read\n  description: >-\n    Read access to the connected Maker account — list and open projects, read\n    project insights, and screenshot previews.\n- name: maker:publish\n  description: >-\n    Publish and mutation access — edit copy, swap images, generate new sections,\n    create variants, set up A/B tests, and push changes live.\ndocs: https://docs.maker.co/features/use-maker-from-your-ai-assistant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makerme/refs/heads/main/scopes/makerme-scopes.yml
summary_line: 2 scopes
tags:
- Company
- A2A
token_bound: false
token_urls: []
---
