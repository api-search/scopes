---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Anthra Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Anthra publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Anthra API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anthra
provider_slug: anthra-com
schemes: []
scope_count: 6
scope_names:
- books:read
- books:write
- generation:run
- publish:write
- account:read
- analytics:read
scopes:
- description: Read books and chapters.
  flows: []
  scope: books:read
- description: Create, update, delete, and outline books and chapters.
  flows: []
  scope: books:write
- description: Run the AI generation pipeline – outline, write, rewrite, narrate.
  flows: []
  scope: generation:run
- description: Publish or unpublish books and change reader visibility.
  flows: []
  scope: publish:write
- description: Read account profile and token usage.
  flows: []
  scope: account:read
- description: Read per‑chapter reader analytics for published books.
  flows: []
  scope: analytics:read
slug: anthra-com-scopes
source_filename: anthra-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://anthra.com/docs/authentication\nscopes:\n  - name: books:read\n    description: Read books and chapters.\n  - name: books:write\n    description: Create, update, delete, and outline books and chapters.\n  - name: generation:run\n    description: Run the AI generation pipeline – outline, write, rewrite, narrate.\n  - name: publish:write\n    description: Publish or unpublish books and change reader visibility.\n  - name: account:read\n    description: Read account profile and token usage.\n  - name: analytics:read\n    description: Read per‑chapter reader analytics for published books.\n"
source_yaml_url: https://artifacts.apis.io/anthra-com/scopes/anthra-com-scopes.yml
summary_line: 6 scopes
tags:
- Artificial Intelligence
- BookCreation
- Writing
- Illustration
- Audiobook
token_bound: false
token_urls: []
---
