---
authorization_urls:
- https://app.getoutline.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Outline Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Outline publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outline API on a user''s behalf.


  Tokens are issued from https://app.getoutline.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outline
provider_slug: outline
schemes:
- flows:
  - authorizationUrl: https://app.getoutline.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.getoutline.com/oauth/token
  name: OAuth2
  source: openapi/outline-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: outline-scopes
source_filename: outline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/outline-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/outline-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getoutline.com/oauth/authorize\n    tokenUrl: https://app.getoutline.com/oauth/token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outline-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/scopes/outline-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Knowledge Base
- Wiki
- Documents
- Collaboration
- Open Source
- Team
token_urls:
- https://app.getoutline.com/oauth/token
---
