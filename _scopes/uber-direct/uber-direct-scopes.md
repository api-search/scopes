---
api_specs:
- filename: uber-direct-openapi.yml
  format: yaml
  label: Uber Direct API
  slug: uber-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-direct/refs/heads/main/openapi/uber-direct-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Uber Direct Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Uber Direct publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Uber Direct API on a user''s behalf.


  Tokens are issued from https://auth.uber.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uber Direct
provider_slug: uber-direct
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.uber.com/oauth/v2/token
  name: oauth2
  source: openapi/uber-direct-openapi.yml
scope_count: 1
scope_names:
- eats.deliveries
scopes:
- description: Access to Uber Direct delivery operations
  flows:
  - clientCredentials
  scope: eats.deliveries
slug: uber-direct-scopes
source_filename: uber-direct-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uber-direct-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/uber-direct-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.uber.com/oauth/v2/token\nscopes:\n- scope: eats.deliveries\n  description: Access to Uber Direct delivery operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-direct-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-direct/refs/heads/main/scopes/uber-direct-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Logistics
- Last Mile Delivery
- Couriers
- Fulfillment
- DaaS
token_urls:
- https://auth.uber.com/oauth/v2/token
---
