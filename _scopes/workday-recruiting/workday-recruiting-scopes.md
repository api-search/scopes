---
authorization_urls:
- https://{tenant}.workday.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Recruiting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Recruiting publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Recruiting API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Recruiting
provider_slug: workday-recruiting
schemes:
- description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting scopes, and obtain access tokens.
  flows:
  - authorizationUrl: https://{tenant}.workday.com/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token
  name: oauth2
  source: openapi/workday-recruiting-rest-api-openapi.yml
scope_count: 2
scope_names:
- recruiting:read
- recruiting:write
scopes:
- description: Read recruiting data
  flows:
  - authorizationCode
  scope: recruiting:read
- description: Modify recruiting data
  flows:
  - authorizationCode
  scope: recruiting:write
slug: workday-recruiting-scopes
source_filename: workday-recruiting-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-recruiting-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-recruiting-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.workday.com/authorize\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token\n  description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting\n    scopes, and obtain access tokens.\nscopes:\n- scope: recruiting:read\n  description: Read recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n- scope: recruiting:write\n  description: Modify recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/scopes/workday-recruiting-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- HCM
- Human Resources
- Recruiting
- SaaS
- Talent Acquisition
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/token
---
