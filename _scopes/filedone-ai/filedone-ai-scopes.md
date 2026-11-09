---
authorization_urls: []
description: ''
docs: https://filedone.ai/developers
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Filedone Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'filedone publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the filedone API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: filedone
provider_slug: filedone-ai
schemes: []
scope_count: 2
scope_names:
- tools:run
- offline_access
scopes:
- description: Call filedone's MCP tools on behalf of the signed-in user. Credit tools debit the user's filedone credits; the assistant is expected to ask get_price and show the cost before running one.
  flows: []
  scope: tools:run
- description: Issue a refresh token so the client can continue to call the MCP server without an interactive sign-in.
  flows: []
  scope: offline_access
slug: filedone-ai-scopes
source_filename: filedone-ai-scopes.yml
source_heading: OAuth Scopes
source_url: https://api.filedone.ai/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://api.filedone.ai/.well-known/oauth-authorization-server\nsources:\n- https://api.filedone.ai/.well-known/oauth-authorization-server\n- https://api.filedone.ai/.well-known/oauth-protected-resource\ndocs: https://filedone.ai/developers\nname: filedone OAuth scopes\nscopes:\n- name: tools:run\n  description: >-\n    Call filedone's MCP tools on behalf of the signed-in user. Credit tools\n    debit the user's filedone credits; the assistant is expected to ask\n    get_price and show the cost before running one.\n- name: offline_access\n  description: >-\n    Issue a refresh token so the client can continue to call the MCP server\n    without an interactive sign-in.\n"
source_yaml_url: https://artifacts.apis.io/filedone-ai/scopes/filedone-ai-scopes.yml
summary_line: 2 scopes
tags:
- PDF
- Image Processing
- Document Conversion
- OCR
- AI Tools
- File Compression
- MCP
- Productivity
token_bound: false
token_urls: []
---
