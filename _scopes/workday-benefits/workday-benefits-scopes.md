---
api_specs:
- filename: Benefits.json
  format: json
  label: Workday Benefits API
  slug: workday-benefits-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Benefits/v40.2/Benefits.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Workday Benefits Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Benefits publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Benefits API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Benefits
provider_slug: workday-benefits
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-openapi.yml
scope_count: 1
scope_names:
- benefits
scopes:
- description: Access to Workday Benefits API
  flows:
  - clientCredentials
  scope: benefits
slug: workday-benefits-scopes
source_filename: workday-benefits-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-benefits-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-benefits-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\nscopes:\n- scope: benefits\n  description: Access to Workday Benefits API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/workday-benefits-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/scopes/workday-benefits-scopes.yml
summary_line: 1 scope · clientCredentials
tags: []
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
---
