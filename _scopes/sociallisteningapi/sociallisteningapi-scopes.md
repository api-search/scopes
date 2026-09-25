---
api_specs:
- filename: sociallisteningapi-openapi.yml
  format: yaml
  label: SocialListeningAPI
  slug: sociallisteningapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-openapi.yml
authorization_urls: []
description: ''
docs: https://sociallisteningapi.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sociallisteningapi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SocialListeningAPI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SocialListeningAPI
provider_slug: sociallisteningapi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sociallisteningapi-scopes
source_filename: sociallisteningapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: https://api.sociallisteningapi.com/.well-known/oauth-protected-resource/mcp (HTTP 200) and /.well-known/oauth-authorization-server\n  (HTTP 200); WWW-Authenticate on POST /mcp names scope=\"mcp\"\ndocs: https://sociallisteningapi.com/mcp\napplies_to: Remote MCP server (the REST API uses an x-api-key header, no scopes)\nscopes:\n- name: mcp\n  description: Scope advertised in scopes_supported and requested in the WWW-Authenticate challenge of the MCP endpoint\n    (no published description).\n- name: mcp:search\n  description: Scope advertised in scopes_supported of the MCP protected-resource and authorization-server metadata\n    (no published description).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/scopes/sociallisteningapi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Social Listening
- Social Media
- Search
- Brand Monitoring
- Market Research
- MCP
- Reddit
- LinkedIn
token_urls: []
---
