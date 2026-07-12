---
authorization_urls:
- https://api.codeproject.com/Authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Codeproject Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CodeProject publishes 1 OAuth 2.0 scope via the clientCredentials, authorizationCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CodeProject API on a user''s behalf.


  Tokens are issued from https://api.codeproject.com/Token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CodeProject
provider_slug: codeproject
schemes:
- description: OAuth 2.0 Bearer Tokens are issued by the CodeProject identity server. Use Client Credentials Grant for read access to public resources and Authorization Code Grant or Implicit Grant for the My API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.codeproject.com/Token
  - authorizationUrl: https://api.codeproject.com/Authorize
    flow: authorizationCode
    tokenUrl: https://api.codeproject.com/Token
  - authorizationUrl: https://api.codeproject.com/Authorize
    flow: implicit
  name: oauth2
  source: openapi/codeproject-rest-api-openapi.yml
scope_count: 1
scope_names:
- read
scopes:
- description: Read access to public resources
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: read
slug: codeproject-scopes
source_filename: codeproject-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codeproject-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/codeproject-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.codeproject.com/Token\n  - flow: authorizationCode\n    authorizationUrl: https://api.codeproject.com/Authorize\n    tokenUrl: https://api.codeproject.com/Token\n  - flow: implicit\n    authorizationUrl: https://api.codeproject.com/Authorize\n  description: OAuth 2.0 Bearer Tokens are issued by the CodeProject identity server. Use Client\n    Credentials Grant for read access to public resources and Authorization Code Grant or Implicit\n    Grant for the My API.\nscopes:\n- scope: read\n  description: Read access to public resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/codeproject-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/scopes/codeproject-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode/implicit
tags:
- AI
- Articles
- Community
- Computer Vision
- Developer Community
- Face Recognition
- Forum
- Knowledge Base
- License Plate Recognition
- Object Detection
- Q&A
- Software Development
- Tutorials
token_urls:
- https://api.codeproject.com/Token
---
