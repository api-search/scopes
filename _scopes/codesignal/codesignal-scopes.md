---
api_specs:
- filename: codesignal-learn-openapi.json
  format: json
  label: CodeSignal Learn Public API
  slug: codesignal-learn-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/openapi/codesignal-learn-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Codesignal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Codesignal publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Codesignal API on a user''s behalf.


  Tokens are issued from https://codesignal.com/learn/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Codesignal
provider_slug: codesignal
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://codesignal.com/learn/api/v1/oauth/token
  name: oauth2
  source: openapi/codesignal-learn-openapi.json
scope_count: 1
scope_names:
- openid
scopes:
- description: basic scope
  flows:
  - clientCredentials
  scope: openid
slug: codesignal-scopes
source_filename: codesignal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/codesignal-learn-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/codesignal-learn-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://codesignal.com/learn/api/v1/oauth/token\nscopes:\n- scope: openid\n  description: basic scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/codesignal-learn-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/scopes/codesignal-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Technical Interview
- Skills Assessment
- Hiring
- Recruiting
- Developer Skills
- Assessment
- Education
- GraphQL
- Webhooks
token_urls:
- https://codesignal.com/learn/api/v1/oauth/token
---
