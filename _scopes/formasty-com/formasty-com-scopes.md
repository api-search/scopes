---
api_specs:
- filename: formasty-com-capabilities-api-openapi.yml
  format: yaml
  label: Formasty Capabilities API
  slug: formasty-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-capabilities-api-openapi.yml
- filename: formasty-com-forms-api-openapi.yml
  format: yaml
  label: Formasty Forms API
  slug: formasty-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-forms-api-openapi.yml
- filename: formasty-com-me-api-openapi.yml
  format: yaml
  label: Formasty Me API
  slug: formasty-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-me-api-openapi.yml
authorization_urls:
- https://app.formasty.com/oauth/authorize/api/v1
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Formasty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Formasty publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Formasty API on a user''s behalf.


  Tokens are issued from https://app.formasty.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Formasty
provider_slug: formasty-com
schemes:
- description: Formasty OAuth authorization-code flow with PKCE and refresh tokens.
  flows:
  - authorizationUrl: https://app.formasty.com/oauth/authorize/api/v1
    flow: authorizationCode
    tokenUrl: https://app.formasty.com/oauth/token
  name: FormastyOAuth
  source: openapi/formasty-com-openapi.json
scope_count: 13
scope_names:
- forms:create
- forms:delete
- forms:design:write
- forms:fields:write
- forms:logic:write
- forms:publish
- forms:read
- forms:steps:write
- forms:update
- submissions:create
- submissions:delete
- submissions:read
- submissions:update
scopes:
- description: Create forms
  flows:
  - authorizationCode
  scope: forms:create
- description: Delete forms
  flows:
  - authorizationCode
  scope: forms:delete
- description: Edit design
  flows:
  - authorizationCode
  scope: forms:design:write
- description: Edit fields
  flows:
  - authorizationCode
  scope: forms:fields:write
- description: Edit logic
  flows:
  - authorizationCode
  scope: forms:logic:write
- description: Publish forms
  flows:
  - authorizationCode
  scope: forms:publish
- description: Read forms
  flows:
  - authorizationCode
  scope: forms:read
- description: Edit steps
  flows:
  - authorizationCode
  scope: forms:steps:write
- description: Update forms
  flows:
  - authorizationCode
  scope: forms:update
- description: Create submissions
  flows:
  - authorizationCode
  scope: submissions:create
- description: Delete submissions
  flows:
  - authorizationCode
  scope: submissions:delete
- description: Read submissions
  flows:
  - authorizationCode
  scope: submissions:read
- description: Update submissions
  flows:
  - authorizationCode
  scope: submissions:update
slug: formasty-com-scopes
source_filename: formasty-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/formasty-com-openapi.json\nschemes:\n- name: FormastyOAuth\n  source: openapi/formasty-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formasty.com/oauth/authorize/api/v1\n    tokenUrl: https://app.formasty.com/oauth/token\n  description: Formasty OAuth authorization-code flow with PKCE and refresh tokens.\nscopes:\n- scope: forms:create\n  description: Create forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:delete\n  description: Delete forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:design:write\n  description: Edit design\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:fields:write\n  description: Edit fields\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:logic:write\n\
  \  description: Edit logic\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:publish\n  description: Publish forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:read\n  description: Read forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:steps:write\n  description: Edit steps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: forms:update\n  description: Update forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: submissions:create\n  description: Create submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: submissions:delete\n  description: Delete submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: submissions:read\n  description: Read\
  \ submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n- scope: submissions:update\n  description: Update submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formasty-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/formasty-com/scopes/formasty-com-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Lead Qualification
- Forms
- Artificial Intelligence
- Automation
- Software-as-a-Service
token_bound: false
token_urls:
- https://app.formasty.com/oauth/token
---
