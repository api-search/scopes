---
authorization_urls:
- https://stackoverflow.com/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Stack Overflow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stack Overflow publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stack Overflow API on a user''s behalf.


  Tokens are issued from https://stackoverflow.com/oauth/access_token/json.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stack Overflow
provider_slug: stack-overflow
schemes:
- description: OAuth 2.0 authentication. Register an application at http://stackapps.com/apps/oauth to obtain credentials.
  flows:
  - authorizationUrl: https://stackoverflow.com/oauth
    flow: authorizationCode
    tokenUrl: https://stackoverflow.com/oauth/access_token/json
  name: oauth2
  source: openapi/stack-overflow-openapi.yml
scope_count: 3
scope_names:
- no_expiry
- private_info
- write_access
scopes:
- description: Issues an access token that does not expire
  flows:
  - authorizationCode
  scope: no_expiry
- description: Access a user's private information
  flows:
  - authorizationCode
  scope: private_info
- description: Allows write access to a user's data
  flows:
  - authorizationCode
  scope: write_access
slug: stack-overflow-scopes
source_filename: stack-overflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stack-overflow-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/stack-overflow-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://stackoverflow.com/oauth\n    tokenUrl: https://stackoverflow.com/oauth/access_token/json\n  description: OAuth 2.0 authentication. Register an application at http://stackapps.com/apps/oauth\n    to obtain credentials.\nscopes:\n- scope: no_expiry\n  description: Issues an access token that does not expire\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stack-overflow-openapi.yml\n- scope: private_info\n  description: Access a user's private information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stack-overflow-openapi.yml\n- scope: write_access\n  description: Allows write access to a user's data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stack-overflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-overflow/refs/heads/main/scopes/stack-overflow-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Answers
- Code
- Developer Community
- Developer Tools
- Knowledge Base
- Programming
- Q&A
- Questions
- Stack Overflow
token_urls:
- https://stackoverflow.com/oauth/access_token/json
---
