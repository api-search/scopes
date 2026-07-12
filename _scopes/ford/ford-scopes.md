---
authorization_urls:
- https://fordconnect.cv.ford.com/common/login
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ford Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ford publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ford API on a user''s behalf.


  Tokens are issued from https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ford
provider_slug: ford
schemes:
- description: OAuth 2.0 authorization-code grant brokered through Ford's identity service
  flows:
  - authorizationUrl: https://fordconnect.cv.ford.com/common/login
    flow: authorizationCode
    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token
  name: oauth2
  source: openapi/ford-openapi.yml
scope_count: 1
scope_names:
- access
scopes:
- description: Access enrolled vehicles
  flows:
  - authorizationCode
  scope: access
slug: ford-scopes
source_filename: ford-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ford-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ford-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fordconnect.cv.ford.com/common/login\n    tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token\n  description: OAuth 2.0 authorization-code grant brokered through Ford's identity service\nscopes:\n- scope: access\n  description: Access enrolled vehicles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ford-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/scopes/ford-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Automobiles
- Cars
- Vehicles
token_urls:
- https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/oauth2/v2.0/token
---
