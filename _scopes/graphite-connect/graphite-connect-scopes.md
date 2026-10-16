---
api_specs:
- filename: graphite-connect-openapi-generated.yml
  format: yaml
  label: Graphite Connect API
  slug: graphite-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/openapi/_ae-authored/graphite-connect-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Graphite Connect Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Graphite Connect publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Graphite Connect API on a user''s behalf.


  Tokens are issued from https://app.graphiteconnect.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Graphite Connect
provider_slug: graphite-connect
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.graphiteconnect.com/api/oauth/token
  name: OAuth_2.0_Client_Credentials
  source: openapi/graphite-connect-openapi-generated.yml
scope_count: 1
scope_names:
- default
scopes:
- description: No scopes defined in provider contract
  flows: []
  scope: default
slug: graphite-connect-scopes
source_filename: graphite-connect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/graphite-connect-openapi-generated.yml\nschemes:\n- name: OAuth_2.0_Client_Credentials\n  source: openapi/graphite-connect-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.graphiteconnect.com/api/oauth/token\nscopes:\n- name: default\n  description: No scopes defined in provider contract\n  source: openapi/_ae-authored/graphite-connect-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/scopes/graphite-connect-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Supplier Management
- Procurement
- AI
- Risk Management
token_bound: false
token_urls:
- https://app.graphiteconnect.com/api/oauth/token
---
