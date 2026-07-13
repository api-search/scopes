---
api_specs:
- filename: unbounce-openapi.yml
  format: yaml
  label: Unbounce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-openapi.yml
authorization_urls:
- https://api.unbounce.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Unbounce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unbounce publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unbounce API on a user''s behalf.


  Tokens are issued from https://api.unbounce.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unbounce
provider_slug: unbounce
schemes:
- description: OAuth 2.0 Authorization Code (granted case-by-case by Unbounce).
  flows:
  - authorizationUrl: https://api.unbounce.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.unbounce.com/oauth/token
  name: oauth2
  source: openapi/unbounce-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to account resources
  flows:
  - authorizationCode
  scope: read
- description: Write access to account resources
  flows:
  - authorizationCode
  scope: write
slug: unbounce-scopes
source_filename: unbounce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unbounce-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/unbounce-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.unbounce.com/oauth/authorize\n    tokenUrl: https://api.unbounce.com/oauth/token\n  description: OAuth 2.0 Authorization Code (granted case-by-case by Unbounce).\nscopes:\n- scope: read\n  description: Read access to account resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unbounce-openapi.yml\n- scope: write\n  description: Write access to account resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unbounce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/scopes/unbounce-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Landing Pages
- Conversion Rate Optimization
- Marketing
- A/B Testing
- Lead Generation
- Marketing Automation
token_urls:
- https://api.unbounce.com/oauth/token
---
