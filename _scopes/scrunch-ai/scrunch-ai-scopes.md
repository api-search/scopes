---
api_specs:
- filename: scrunch-ai-data-api-openapi.yml
  format: yaml
  label: Scrunch Data API
  slug: scrunch-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-data-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.scrunch.com/getting-started/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Scrunch Ai Scopes
name_suffix: OAuth Scopes
note: Scrunch does not use OAuth2 authorization flows for the Data API - scopes are attached to organization-level API keys (Bearer tokens) at creation time and enforced per operation via the HTTPBearer security scheme. These are the operational scopes the OpenAPI security requirements reference and that the docs document as selectable key scopes. (The separate hosted MCP server uses OAuth sign-in - see mcp/scrunch-ai-mcp.yml.)
overview: 'Scrunch AI publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Scrunch AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scrunch AI
provider_slug: scrunch-ai
schemes: []
scope_count: 3
scope_names:
- query
- configure
- create-brand
scopes:
- description: Retrieve analytics and metrics (Query, Responses, Sitemap, Agent Traffic reads).
  flows: []
  scope: query
- description: Update brand configuration - brands, competitors, personas, prompts, page audits.
  flows: []
  scope: configure
- description: Programmatically create new brands.
  flows: []
  scope: create-brand
slug: scrunch-ai-scopes
source_filename: scrunch-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scrunch-ai-data-api-openapi.yml\ndocs: https://developers.scrunch.com/getting-started/authentication\nmodel: api-key-scopes\nnote: |\n  Scrunch does not use OAuth2 authorization flows for the Data API - scopes are attached\n  to organization-level API keys (Bearer tokens) at creation time and enforced per\n  operation via the HTTPBearer security scheme. These are the operational scopes the\n  OpenAPI security requirements reference and that the docs document as selectable key\n  scopes. (The separate hosted MCP server uses OAuth sign-in - see mcp/scrunch-ai-mcp.yml.)\nscheme: HTTPBearer\nscopes:\n- scope: query\n  description: Retrieve analytics and metrics (Query, Responses, Sitemap, Agent Traffic reads).\n- scope: configure\n  description: Update brand configuration - brands, competitors, personas, prompts, page audits.\n- scope: create-brand\n  description: Programmatically create new brands.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/scopes/scrunch-ai-scopes.yml
summary_line: 3 scopes
tags:
- Company
- AI
- AI Search
- Answer Engine Optimization
- Generative Engine Optimization
- Brand Visibility
- Analytics
- SEO
- Agent Experience
- MCP
token_urls: []
---
