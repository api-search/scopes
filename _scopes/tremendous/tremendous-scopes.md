---
authorization_urls:
- https://www.tremendous.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Tremendous Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tremendous publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tremendous API on a user''s behalf.


  Tokens are issued from https://www.tremendous.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tremendous
provider_slug: tremendous
schemes:
- description: OAuth 2.0 for third-party integrations
  flows:
  - authorizationUrl: https://www.tremendous.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.tremendous.com/oauth/token
  name: OAuth2
  source: openapi/tremendous-api-openapi.yml
scope_count: 3
scope_names:
- manage
- read
- write
scopes:
- description: Manage organization settings, members, and webhooks
  flows:
  - authorizationCode
  scope: manage
- description: Read access to orders, rewards, products, and funding sources
  flows:
  - authorizationCode
  scope: read
- description: Create orders and rewards
  flows:
  - authorizationCode
  scope: write
slug: tremendous-scopes
source_filename: tremendous-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tremendous-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/tremendous-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tremendous.com/oauth/authorize\n    tokenUrl: https://www.tremendous.com/oauth/token\n  description: OAuth 2.0 for third-party integrations\nscopes:\n- scope: manage\n  description: Manage organization settings, members, and webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tremendous-api-openapi.yml\n- scope: read\n  description: Read access to orders, rewards, products, and funding sources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tremendous-api-openapi.yml\n- scope: write\n  description: Create orders and rewards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tremendous-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremendous/refs/heads/main/scopes/tremendous-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Employee Incentives
- Global Payouts
- Incentives
- Market Research
- Payouts
- Rewards
token_urls:
- https://www.tremendous.com/oauth/token
---
