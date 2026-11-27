---
api_specs:
- filename: chikoh-com-contest-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Contest Intelligence API
  slug: chikoh-com-contest-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-contest-intelligence-api-openapi.yml
- filename: chikoh-com-entertainment-api-openapi.yml
  format: yaml
  label: Chikoh Entertainment API
  slug: chikoh-com-entertainment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-entertainment-api-openapi.yml
- filename: chikoh-com-entertainment-predictions-api-openapi.yml
  format: yaml
  label: Chikoh Entertainment Predictions API
  slug: chikoh-com-entertainment-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-entertainment-predictions-api-openapi.yml
- filename: chikoh-com-market-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Market Intelligence API
  slug: chikoh-com-market-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-market-intelligence-api-openapi.yml
- filename: chikoh-com-player-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Player Intelligence API
  slug: chikoh-com-player-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-player-intelligence-api-openapi.yml
- filename: chikoh-com-strategic-intelligence-api-openapi.yml
  format: yaml
  label: Chikoh Strategic Intelligence API
  slug: chikoh-com-strategic-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chikoh-com/openapi/chikoh-com-strategic-intelligence-api-openapi.yml
authorization_urls:
- https://chikoh.com/api/v1/oauth/authorize
description: ''
docs: https://chikoh.com/developers
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Chikoh Scopes
name_suffix: OAuth Scopes
note: 'The developers page GPT Action setup documents "Scope: read"; the syndicate scope appears only in the OpenAPI securitySchemes.'
overview: 'Chikoh publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chikoh API on a user''s behalf.


  Tokens are issued from https://chikoh.com/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chikoh
provider_slug: chikoh-com
schemes:
- description: Sign in with your Chikoh account. Required for Syndicate tools.
  flows:
  - authorizationUrl: https://chikoh.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://chikoh.com/api/v1/oauth/token
  name: oauth2
  source: openapi/chikoh-com-openapi.yml
scope_count: 2
scope_names:
- read
- syndicate
scopes:
- description: Access all free and authenticated tools
  flows:
  - authorizationCode
  scope: read
- description: Access Syndicate-exclusive whale tools (requires The Syndicate tier)
  flows:
  - authorizationCode
  scope: syndicate
slug: chikoh-com-scopes
source_filename: chikoh-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chikoh.com/developers\nschemes:\n- name: oauth2\n  source: openapi/chikoh-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://chikoh.com/api/v1/oauth/authorize\n    tokenUrl: https://chikoh.com/api/v1/oauth/token\n  description: Sign in with your Chikoh account. Required for Syndicate tools.\nscopes:\n- scope: read\n  description: Access all free and authenticated tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chikoh-com-openapi.yml\n- scope: syndicate\n  description: Access Syndicate-exclusive whale tools (requires The Syndicate tier)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chikoh-com-openapi.yml\ndocs: https://chikoh.com/developers\nnote: 'The developers page GPT Action setup documents \"Scope: read\"; the syndicate scope appears only in the OpenAPI securitySchemes.'\n"
source_yaml_url: https://artifacts.apis.io/chikoh-com/scopes/chikoh-com-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fantasy Sports
- Sports Analytics
- Reality TV
- Predictions
- Gaming
- AI Agents
- MCP
token_bound: false
token_urls:
- https://chikoh.com/api/v1/oauth/token
---
