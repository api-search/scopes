---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Workday Business Processes Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Business Processes publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Business Processes API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Business Processes
provider_slug: workday-business-processes
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-business-processes-openapi.yml
scope_count: 1
scope_names:
- businessProcess
scopes:
- description: Access to Workday Business Process API
  flows:
  - clientCredentials
  scope: businessProcess
slug: workday-business-processes-scopes
source_filename: workday-business-processes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-business-processes-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-business-processes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\nscopes:\n- scope: businessProcess\n  description: Access to Workday Business Process API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/workday-business-processes-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/scopes/workday-business-processes-scopes.yml
summary_line: 1 scope · clientCredentials
tags: []
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
---
