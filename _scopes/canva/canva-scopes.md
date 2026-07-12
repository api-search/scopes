---
authorization_urls:
- https://www.canva.com/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Canva Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canva publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canva API on a user''s behalf.


  Tokens are issued from https://api.canva.com/rest/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canva
provider_slug: canva
schemes:
- description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included in the Authorization header as a Bearer token.
  flows:
  - authorizationUrl: https://www.canva.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.canva.com/rest/v1/oauth/token
  name: oauth2
  source: openapi/canva-connect-api-openapi.yml
scope_count: 11
scope_names:
- asset:read
- asset:write
- brandtemplate:content:read
- brandtemplate:meta:read
- comment:read
- comment:write
- design:content:read
- design:content:write
- design:meta:read
- folder:read
- folder:write
scopes:
- description: Read asset metadata
  flows:
  - authorizationCode
  scope: asset:read
- description: Upload and delete assets
  flows:
  - authorizationCode
  scope: asset:write
- description: Read brand template content and datasets
  flows:
  - authorizationCode
  scope: brandtemplate:content:read
- description: Read brand template metadata
  flows:
  - authorizationCode
  scope: brandtemplate:meta:read
- description: Read comments on designs
  flows:
  - authorizationCode
  scope: comment:read
- description: Create and manage comments
  flows:
  - authorizationCode
  scope: comment:write
- description: Read design content
  flows:
  - authorizationCode
  scope: design:content:read
- description: Create and modify designs
  flows:
  - authorizationCode
  scope: design:content:write
- description: Read design metadata
  flows:
  - authorizationCode
  scope: design:meta:read
- description: Read folder metadata and contents
  flows:
  - authorizationCode
  scope: folder:read
- description: Modify folder contents
  flows:
  - authorizationCode
  scope: folder:write
slug: canva-scopes
source_filename: canva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canva-connect-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/canva-connect-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.canva.com/api/oauth/authorize\n    tokenUrl: https://api.canva.com/rest/v1/oauth/token\n  description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included\n    in the Authorization header as a Bearer token.\nscopes:\n- scope: asset:read\n  description: Read asset metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: asset:write\n  description: Upload and delete assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: brandtemplate:content:read\n  description: Read brand template content and datasets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: brandtemplate:meta:read\n\
  \  description: Read brand template metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: comment:read\n  description: Read comments on designs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: comment:write\n  description: Create and manage comments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: design:content:read\n  description: Read design content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: design:content:write\n  description: Create and modify designs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: design:meta:read\n  description: Read design metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: folder:read\n  description: Read folder metadata and contents\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/canva-connect-api-openapi.yml\n- scope: folder:write\n  description: Modify folder contents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canva-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/scopes/canva-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
token_urls:
- https://api.canva.com/rest/v1/oauth/token
---
