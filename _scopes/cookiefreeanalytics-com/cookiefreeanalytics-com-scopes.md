---
api_specs:
- filename: cookiefreeanalytics-com-sites-api-openapi.yml
  format: yaml
  label: Cookie Free Analytics Sites API
  slug: cookiefreeanalytics-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiefreeanalytics-com/openapi/cookiefreeanalytics-com-sites-api-openapi.yml
authorization_urls: []
description: Scopes advertised in the RFC 9728 protected-resource metadata for the MCP endpoint (GET, HTTP 200). The OpenAPI contract declares only a bearer scheme and no OAuth scopes; the docs do not publish per-scope descriptions, so none are given beyond the scope names.
docs: https://www.cookiefreeanalytics.com/docs/api
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cookie Free Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cookie Free Analytics publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cookie Free Analytics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cookie Free Analytics
provider_slug: cookiefreeanalytics-com
schemes:
- name: mcp-oauth
scope_count: 2
scope_names:
- analytics:read
- sites:write
scopes:
- description: ''
  flows: []
  scope: analytics:read
- description: ''
  flows: []
  scope: sites:write
slug: cookiefreeanalytics-com-scopes
source_filename: cookiefreeanalytics-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://www.cookiefreeanalytics.com/.well-known/oauth-protected-resource\ndocs: https://www.cookiefreeanalytics.com/docs/api\ndescription: Scopes advertised in the RFC 9728 protected-resource metadata for the MCP endpoint (GET, HTTP 200). The OpenAPI contract declares only a bearer scheme and no OAuth scopes; the docs do not publish per-scope descriptions, so none are given beyond the scope names.\nschemes:\n- name: mcp-oauth\nscopes:\n- scope: analytics:read\n  schemes:\n  - mcp-oauth\n- scope: sites:write\n  schemes:\n  - mcp-oauth\n"
source_yaml_url: https://artifacts.apis.io/cookiefreeanalytics-com/scopes/cookiefreeanalytics-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
- MCP
- Uptime Monitoring
token_bound: false
token_urls: []
---
