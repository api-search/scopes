---
api_specs:
- filename: rest-api-spec
  format: yaml
  label: Figma REST API
  slug: figma-api
  spec_type: OpenAPI
  url: https://github.com/figma/rest-api-spec
authorization_urls:
- https://www.figma.com/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wireframes Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wireframes publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wireframes API on a user''s behalf.


  Tokens are issued from https://api.figma.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wireframes
provider_slug: wireframes
schemes:
- description: OAuth 2.0 authentication for registered applications
  flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: oauth2
  source: openapi/wireframes-openapi.yml
scope_count: 2
scope_names:
- file_comments:write
- files:read
scopes:
- description: Write file comments
  flows:
  - authorizationCode
  scope: file_comments:write
- description: Read files
  flows:
  - authorizationCode
  scope: files:read
slug: wireframes-scopes
source_filename: wireframes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wireframes-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wireframes-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n  description: OAuth 2.0 authentication for registered applications\nscopes:\n- scope: file_comments:write\n  description: Write file comments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wireframes-openapi.yml\n- scope: files:read\n  description: Read files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wireframes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wireframes/refs/heads/main/scopes/wireframes-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Design
- Figma
- Prototyping
- UI Design
- UX
- Wireframing
token_urls:
- https://api.figma.com/v1/oauth/token
---
