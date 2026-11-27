---
api_specs:
- filename: aislesinventory-com-agent-api-openapi.yml
  format: yaml
  label: Aisles Inc. Agent API
  slug: aislesinventory-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-agent-api-openapi.yml
- filename: aislesinventory-com-jobs-api-openapi.yml
  format: yaml
  label: Aisles Inc. Jobs API
  slug: aislesinventory-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-jobs-api-openapi.yml
- filename: aislesinventory-com-sandbox-api-openapi.yml
  format: yaml
  label: Aisles Inc. Sandbox API
  slug: aislesinventory-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-sandbox-api-openapi.yml
- filename: aislesinventory-com-search-api-openapi.yml
  format: yaml
  label: Aisles Inc. Search API
  slug: aislesinventory-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-search-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Aisles Inc. Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aisles Inc. publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aisles Inc. API on a user''s behalf.


  Tokens are issued from https://aislesinventory.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aisles Inc.
provider_slug: aislesinventory-com
schemes:
- description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register, then client credentials.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://aislesinventory.com/oauth/token
  name: oauth2
  source: openapi/aislesinventory-com-openapi.json
- description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register, then client credentials.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://aislesinventory.com/oauth/token
  name: oauth2
  source: openapi/aislesinventory-com-sandbox-openapi.json
scope_count: 2
scope_names:
- read:answers
- read:inventory
scopes:
- description: Read the ready answers per city
  flows:
  - clientCredentials
  scope: read:answers
- description: Search store stock
  flows:
  - clientCredentials
  scope: read:inventory
slug: aislesinventory-com-scopes
source_filename: aislesinventory-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/aislesinventory-com-openapi.json, openapi/aislesinventory-com-sandbox-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/aislesinventory-com-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://aislesinventory.com/oauth/token\n  description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register,\n    then client credentials.'\n- name: oauth2\n  source: openapi/aislesinventory-com-sandbox-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://aislesinventory.com/oauth/token\n  description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register,\n    then client credentials.'\nscopes:\n- scope: read:answers\n  description: Read the ready answers per city\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aislesinventory-com-openapi.json\n  - openapi/aislesinventory-com-sandbox-openapi.json\n\
  - scope: read:inventory\n  description: Search store stock\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aislesinventory-com-openapi.json\n  - openapi/aislesinventory-com-sandbox-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aislesinventory-com/scopes/aislesinventory-com-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Inventory
- Retail
- Stocks
- US
token_bound: false
token_urls:
- https://aislesinventory.com/oauth/token
---
