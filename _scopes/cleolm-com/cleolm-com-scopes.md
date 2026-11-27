---
api_specs:
- filename: cleolm-com-tools-api-openapi.yml
  format: yaml
  label: CleoLM Tools API
  slug: cleolm-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleolm-com/openapi/cleolm-com-tools-api-openapi.yml
authorization_urls:
- https://cleolm.com/oauth/authorize
description: ''
docs: https://cleolm.com/developers
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: CleoLM Scopes
name_suffix: OAuth Scopes
note: API keys are not OAuth-scoped by name, but the docs state keys "can be scoped to exclude ingest" (Allow ingest checkbox on /developers), mirroring the cleolm.ingest scope.
overview: 'CleoLM publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CleoLM API on a user''s behalf.


  Tokens are issued from https://cleolm.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CleoLM
provider_slug: cleolm-com
schemes:
- flows:
  - authorizationUrl: https://cleolm.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://cleolm.com/oauth/token
  name: oauth2
  source: openapi/cleolm-com-openapi.yml
scope_count: 2
scope_names:
- cleolm.ingest
- cleolm.read
scopes:
- description: Transcribe new videos and podcasts using your plan's credits
  flows:
  - authorizationCode
  scope: cleolm.ingest
- description: Search the CleoLM index and your library, and read transcripts
  flows:
  - authorizationCode
  scope: cleolm.read
slug: cleolm-com-scopes
source_filename: cleolm-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cleolm.com/llms.txt\nschemes:\n- name: oauth2\n  source: openapi/cleolm-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cleolm.com/oauth/authorize\n    tokenUrl: https://cleolm.com/oauth/token\nscopes:\n- scope: cleolm.ingest\n  description: Transcribe new videos and podcasts using your plan's credits\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cleolm-com-openapi.yml\n- scope: cleolm.read\n  description: Search the CleoLM index and your library, and read transcripts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cleolm-com-openapi.yml\ndocs: https://cleolm.com/developers\nnote: API keys are not OAuth-scoped by name, but the docs state keys \"can be scoped\n  to exclude ingest\" (Allow ingest checkbox on /developers), mirroring the cleolm.ingest\n  scope.\n"
source_yaml_url: https://artifacts.apis.io/cleolm-com/scopes/cleolm-com-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Transcription
- Podcasts
- YouTube
- Search
- MCP
- Video
token_bound: false
token_urls:
- https://cleolm.com/oauth/token
---
