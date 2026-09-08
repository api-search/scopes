---
api_specs:
- filename: perfect-corp-ai_abs_filter-openapi.yml
  format: yaml
  label: YouCam AI REST API
  slug: youcam-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/openapi/perfect-corp-ai_abs_filter-openapi.yml
authorization_urls: []
description: The 65 published OpenAPI documents declare only HTTP bearer security, so nothing OAuth-shaped is derivable from the contracts. The OAuth surface is discoverable instead at the RFC 8414 Authorization Server Metadata document the API host serves anonymously, which names two scopes. Perfect Corp's prose documentation describes only the API-key bearer flow and does not document these scopes anywhere, so this artifact is the only public record of them.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Perfect Corp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Perfect Corp uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Perfect Corp
provider_slug: perfect-corp
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: perfect-corp-scopes
source_filename: perfect-corp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server\nname: Perfect Corp YouCam API — OAuth 2.0 scopes\ndescription: >-\n  The 65 published OpenAPI documents declare only HTTP bearer security, so nothing OAuth-shaped is\n  derivable from the contracts. The OAuth surface is discoverable instead at the RFC 8414\n  Authorization Server Metadata document the API host serves anonymously, which names two scopes.\n  Perfect Corp's prose documentation describes only the API-key bearer flow and does not document\n  these scopes anywhere, so this artifact is the only public record of them.\ndocs: null\ndocs_note: >-\n  No scopes / permissions reference page exists in the developer documentation. The scope names below\n  come from the machine-readable metadata document, not from prose.\n\nauthorization_server:\n  issuer: https://yce-api-01.perfectcorp.com\n  metadata_url: https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server\n\
  \  metadata_file: well-known/perfect-corp-oauth-authorization-server.json\n  authorization_endpoint: https://yce-api-01.perfectcorp.com/oauth2/authorize\n  token_endpoint: https://yce-api-01.perfectcorp.com/oauth2/token\n  registration_endpoint: https://yce-api-01.perfectcorp.com/oauth2/register\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  note: >-\n    A public-client profile — PKCE S256 mandatory, no client secret at the token endpoint, dynamic\n    client registration (RFC 7591) open, and RFC 9728-style client-id metadata documents supported.\n    That combination is the shape an MCP/agent client needs; the hosted MCP servers nonetheless\n    authenticate with a static API key today and serve no /.well-known/oauth-protected-resource.\n\nscope_count: 2\nscopes:\n  - name: task.run\n    description:\
  \ >-\n      Create and execute AI tasks. Inferred usage: the write half of the API — POST /s2s/v2.x/task/*\n      and POST /s2s/v2.0/file. Perfect Corp publishes no scope description; the name is verbatim from\n      scopes_supported.\n    grants: write\n  - name: task.read\n    description: >-\n      Read task status and results. Inferred usage: GET /s2s/v2.x/task/*/{task_id} and the unit /\n      feature-cost reads. Perfect Corp publishes no scope description; the name is verbatim from\n      scopes_supported.\n    grants: read\n\nx-evidence:\n  - url: https://yce-api-01.makeupar.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n    fetched: '2026-09-02'\n  - url: https://yce-api-01.perfectcorp.com/.well-known/oauth-authorization-server\n    http_status: 200\n    note: The issuer host serves the identical document.\n  - url: https://mcp-api-01.makeupar.com/.well-known/oauth-authorization-server\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfect-corp/refs/heads/main/scopes/perfect-corp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- beauty
- skincare
- cosmetics
- fashion
- apparel
- jewelry
- watches
- hair
- virtual-try-on
- image-editing
- generative-ai
- computer-vision
- AR
- visual-commerce
- ai
- machine-learning
- video-generation
- skin-analysis
- mcp
- agents
- photo-editing
- beauty-tech
- retail
- ar-try-on
token_urls: []
---
