---
api_specs:
- filename: aiapplyd-openapi.yml
  format: yaml
  label: AI Applyd API
  slug: ai-applyd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/openapi/aiapplyd-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aiapplyd Scopes
name_suffix: OAuth Scopes
note: Only OpenID Connect identity scopes are advertised; no product-level permission scopes are published.
overview: 'AI Applyd uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AI Applyd
provider_slug: aiapplyd
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aiapplyd-scopes
source_filename: aiapplyd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource:\n- https://mcp.aiapplyd.com/.well-known/oauth-protected-resource\n- https://mcp.aiapplyd.com/.well-known/oauth-authorization-server\nscopes:\n- name: openid\n  api: AI Applyd MCP Server\n- name: email\n  api: AI Applyd MCP Server\n- name: profile\n  api: AI Applyd MCP Server\n- name: offline_access\n  api: AI Applyd MCP Server\nnote: Only OpenID Connect identity scopes are advertised; no product-level permission scopes are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiapplyd/refs/heads/main/scopes/aiapplyd-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Job Search
- Recruiting
- Resume
- Applicant Tracking Systems
- Careers
- Artificial Intelligence
- MCP
- Automation
token_urls: []
---
