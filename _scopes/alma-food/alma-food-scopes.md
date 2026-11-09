---
api_specs:
- filename: alma-food-discovery-api-openapi.yml
  format: yaml
  label: Alma Discovery API
  slug: alma-food-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alma-food/openapi/alma-food-discovery-api-openapi.yml
authorization_urls:
- https://mcp.alma.food/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Alma Food Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alma publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alma API on a user''s behalf.


  Tokens are issued from https://mcp.alma.food/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alma
provider_slug: alma-food
schemes:
- description: OAuth for the Alma MCP server at https://mcp.alma.food. Request only the scopes needed for the job.
  flows:
  - authorizationUrl: https://mcp.alma.food/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.alma.food/token
  name: almaMcpOAuth
  source: openapi/alma-food-openapi.json
scope_count: 2
scope_names:
- alma:read
- alma:write
scopes:
- description: Read a member's authorized nutrition data (meals, Alma Score, goals, weight, profile).
  flows:
  - authorizationCode
  scope: alma:read
- description: Write access if the member authorizes it.
  flows:
  - authorizationCode
  scope: alma:write
slug: alma-food-scopes
source_filename: alma-food-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/alma-food-openapi.json\nschemes:\n- name: almaMcpOAuth\n  source: openapi/alma-food-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.alma.food/authorize\n    tokenUrl: https://mcp.alma.food/token\n  description: OAuth for the Alma MCP server at https://mcp.alma.food. Request only the scopes\n    needed for the job.\nscopes:\n- scope: alma:read\n  description: Read a member's authorized nutrition data (meals, Alma Score, goals, weight,\n    profile).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/alma-food-openapi.json\n- scope: alma:write\n  description: Write access if the member authorizes it.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/alma-food-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alma-food/scopes/alma-food-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Nutrition
- Artificial Intelligence
- Health
- Food Tracking
- Personalization
- Company
token_bound: false
token_urls:
- https://mcp.alma.food/token
---
