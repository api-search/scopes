---
api_specs:
- filename: kadence-public-api-openapi.yml
  format: yaml
  label: Kadence Public API
  slug: kadence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-public-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Kadence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kadence publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kadence API on a user''s behalf.


  Tokens are issued from https://login.onkadence.co/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kadence
provider_slug: kadence
schemes:
- description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.onkadence.co/oauth2/token
  name: oauth
  source: openapi/kadence-public-api-openapi.yml
scope_count: 1
scope_names:
- public
scopes:
- description: Public API access
  flows:
  - clientCredentials
  scope: public
slug: kadence-scopes
source_filename: kadence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kadence-public-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/kadence-public-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.onkadence.co/oauth2/token\n  description: OAuth 2.0 client credentials Grant\nscopes:\n- scope: public\n  description: Public API access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kadence-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/scopes/kadence-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- OAuth
token_urls:
- https://login.onkadence.co/oauth2/token
---
