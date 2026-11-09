---
api_specs:
- filename: steamgpt-net-bans-api-openapi.yml
  format: yaml
  label: steamgpt-net Bans API
  slug: steamgpt-net-bans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-bans-api-openapi.yml
- filename: steamgpt-net-batch-api-openapi.yml
  format: yaml
  label: steamgpt-net Batch API
  slug: steamgpt-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-batch-api-openapi.yml
- filename: steamgpt-net-compare-api-openapi.yml
  format: yaml
  label: steamgpt-net Compare API
  slug: steamgpt-net-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-compare-api-openapi.yml
- filename: steamgpt-net-converter-api-openapi.yml
  format: yaml
  label: steamgpt-net Converter API
  slug: steamgpt-net-converter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-converter-api-openapi.yml
- filename: steamgpt-net-faceit-api-openapi.yml
  format: yaml
  label: steamgpt-net Faceit API
  slug: steamgpt-net-faceit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-faceit-api-openapi.yml
- filename: steamgpt-net-friends-api-openapi.yml
  format: yaml
  label: steamgpt-net Friends API
  slug: steamgpt-net-friends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-friends-api-openapi.yml
- filename: steamgpt-net-identity-api-openapi.yml
  format: yaml
  label: steamgpt-net Identity API
  slug: steamgpt-net-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-identity-api-openapi.yml
- filename: steamgpt-net-profile-api-openapi.yml
  format: yaml
  label: steamgpt-net Profile API
  slug: steamgpt-net-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-profile-api-openapi.yml
- filename: steamgpt-net-ready-api-openapi.yml
  format: yaml
  label: steamgpt-net Ready API
  slug: steamgpt-net-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-ready-api-openapi.yml
- filename: steamgpt-net-summary-api-openapi.yml
  format: yaml
  label: steamgpt-net Summary API
  slug: steamgpt-net-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-summary-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Steamgpt Net Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'steamgpt-net publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the steamgpt-net API on a user''s behalf.


  Tokens are issued from https://steamgpt.net/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: steamgpt-net
provider_slug: steamgpt-net
schemes:
- description: 'OPTIONAL. Every endpoint works without any credential. A self-service token (no registration, no client_id) raises the per-IP rate limit from 120 to 600 requests/min. Send it as: Authorization: Bearer <access_token>. Details: https://steamgpt.net/auth.md'
  flows:
  - flow: clientCredentials
    tokenUrl: https://steamgpt.net/oauth/token
  name: boostToken
  source: openapi/steamgpt-net-openapi.json
scope_count: 1
scope_names:
- rate-boost
scopes:
- description: Higher per-IP rate limit (600/min instead of 120/min)
  flows:
  - clientCredentials
  scope: rate-boost
slug: steamgpt-net-scopes
source_filename: steamgpt-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/steamgpt-net-openapi.json\nschemes:\n- name: boostToken\n  source: openapi/steamgpt-net-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://steamgpt.net/oauth/token\n  description: 'OPTIONAL. Every endpoint works without any credential. A self-service token\n    (no registration, no client_id) raises the per-IP rate limit from 120 to 600 requests/min.\n    Send it as: Authorization: Bearer <access_token>. Details: https://steamgpt.net/auth.md'\nscopes:\n- scope: rate-boost\n  description: Higher per-IP rate limit (600/min instead of 120/min)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/steamgpt-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/steamgpt-net/scopes/steamgpt-net-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Artificial Intelligence
- Gaming
- Steam
token_bound: false
token_urls:
- https://steamgpt.net/oauth/token
---
