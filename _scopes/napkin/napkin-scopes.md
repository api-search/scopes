---
api_specs:
- filename: napkin-openapi.yml
  format: yaml
  label: Napkin API
  slug: napkin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkin/refs/heads/main/openapi/napkin-openapi.yml
authorization_urls:
- https://api.napkin.ai/v1/oauth/authorize
description: ''
docs: https://api.napkin.ai/oauth-user-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Napkin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Napkin publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Napkin API on a user''s behalf.


  Tokens are issued from https://api.napkin.ai/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Napkin
provider_slug: napkin
schemes:
- flows:
  - authorizationUrl: https://api.napkin.ai/v1/oauth/authorize
    flow: authorizationCode
    revokeUrl: https://api.napkin.ai/v1/oauth/revoke
    tokenUrl: https://api.napkin.ai/v1/oauth/token
  name: oauth2
  source: openapi/napkin-openapi.yml
scope_count: 2
scope_names:
- user
- generation
scopes:
- description: Access to basic user profile information (email, name, user ID).
  flows:
  - authorizationCode
  scope: user
- description: Ability to create visual generations on behalf of the user.
  flows:
  - authorizationCode
  scope: generation
slug: napkin-scopes
source_filename: napkin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/napkin-openapi.yml\ndocs: https://api.napkin.ai/oauth-user-authentication\nschemes:\n  - name: oauth2\n    source: openapi/napkin-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.napkin.ai/v1/oauth/authorize\n        tokenUrl: https://api.napkin.ai/v1/oauth/token\n        revokeUrl: https://api.napkin.ai/v1/oauth/revoke\nscopes:\n  - scope: user\n    description: Access to basic user profile information (email, name, user ID).\n    flows: [authorizationCode]\n    sources: [openapi/napkin-openapi.yml]\n  - scope: generation\n    description: Ability to create visual generations on behalf of the user.\n    flows: [authorizationCode]\n    sources: [openapi/napkin-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkin/refs/heads/main/scopes/napkin-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Ai
- Visualization
- Diagrams
- Infographics
- Presentations
- Content Generation
- Developer API
- Design
token_urls:
- https://api.napkin.ai/v1/oauth/token
---
