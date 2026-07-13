---
api_specs:
- filename: swagger
  format: yaml
  label: Getty Images API
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Getty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Getty Images publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Getty Images API on a user''s behalf.


  Tokens are issued from https://api.gettyimages.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Getty Images
provider_slug: getty
schemes:
- description: OAuth 2.0 client credentials for elevated operations.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.gettyimages.com/oauth2/token
  name: oauth2
  source: openapi/getty-openapi.yml
scope_count: 2
scope_names:
- download
- read
scopes:
- description: Request download URLs for licensed assets
  flows:
  - clientCredentials
  scope: download
- description: Read access to assets
  flows:
  - clientCredentials
  scope: read
slug: getty-scopes
source_filename: getty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/getty-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/getty-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.gettyimages.com/oauth2/token\n  description: OAuth 2.0 client credentials for elevated operations.\nscopes:\n- scope: download\n  description: Request download URLs for licensed assets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getty-openapi.yml\n- scope: read\n  description: Read access to assets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getty/refs/heads/main/scopes/getty-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Stock Media
- Images
- Editorial
- Video
- Music
- Licensing
token_urls:
- https://api.gettyimages.com/oauth2/token
---
