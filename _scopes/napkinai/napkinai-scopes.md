---
api_specs:
- filename: napkinai-openapi.yml
  format: yaml
  label: Napkin AI API
  slug: napkin-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/openapi/napkinai-openapi.yml
authorization_urls:
- https://api.napkin.ai/v1/oauth/authorize
description: ''
docs: https://api.napkin.ai/oauth-user-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Napkinai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Napkin.AI publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Napkin.AI API on a user''s behalf.


  Tokens are issued from https://api.napkin.ai/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Napkin.AI
provider_slug: napkinai
schemes:
- description: OAuth 2.0 authorization code flow (beta). Your application must be approved by the Napkin AI team to obtain client credentials.
  flows:
  - authorizationUrl: https://api.napkin.ai/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.napkin.ai/v1/oauth/token
  name: oauth2
  source: openapi/napkinai-openapi.yml
scope_count: 2
scope_names:
- generation
- user
scopes:
- description: Ability to create visual generations on behalf of the user
  flows:
  - authorizationCode
  scope: generation
- description: Access to basic user profile information (email, name, user ID)
  flows:
  - authorizationCode
  scope: user
slug: napkinai-scopes
source_filename: napkinai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/napkinai-openapi.yml\ndocs: https://api.napkin.ai/oauth-user-authentication\nschemes:\n- name: oauth2\n  source: openapi/napkinai-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.napkin.ai/v1/oauth/authorize\n    tokenUrl: https://api.napkin.ai/v1/oauth/token\n  description: OAuth 2.0 authorization code flow (beta). Your application must be approved by\n    the Napkin AI team to obtain client credentials.\nscopes:\n- scope: generation\n  description: Ability to create visual generations on behalf of the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/napkinai-openapi.yml\n- scope: user\n  description: Access to basic user profile information (email, name, user ID)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/napkinai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/scopes/napkinai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Ai
- Visualization
- Diagrams
- Charts
- Infographics
- Presentations
- Content Generation
- Design
- Developer API
token_urls:
- https://api.napkin.ai/v1/oauth/token
---
