---
authorization_urls:
- https://runsignup.com/OAuth/Authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Runsignup Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RunSignup publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RunSignup API on a user''s behalf.


  Tokens are issued from https://runsignup.com/OAuth/Token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RunSignup
provider_slug: runsignup
schemes:
- description: OAuth 2.0 authentication (preferred)
  flows:
  - authorizationUrl: https://runsignup.com/OAuth/Authorize
    flow: authorizationCode
    tokenUrl: https://runsignup.com/OAuth/Token
  name: OAuth2
  source: openapi/runsignup-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to race and participant data
  flows:
  - authorizationCode
  scope: read
- description: Write access to race and participant data
  flows:
  - authorizationCode
  scope: write
slug: runsignup-scopes
source_filename: runsignup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runsignup-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/runsignup-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://runsignup.com/OAuth/Authorize\n    tokenUrl: https://runsignup.com/OAuth/Token\n  description: OAuth 2.0 authentication (preferred)\nscopes:\n- scope: read\n  description: Read access to race and participant data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/runsignup-openapi.yml\n- scope: write\n  description: Write access to race and participant data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/runsignup-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runsignup/refs/heads/main/scopes/runsignup-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Race Registration
- Event Management
- Running
- Sports
- Fitness
- Timing
- Fundraising
token_urls:
- https://runsignup.com/OAuth/Token
---
