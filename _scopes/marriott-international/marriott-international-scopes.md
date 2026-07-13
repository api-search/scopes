---
api_specs:
- filename: marriott-international-developer-api-openapi.yml
  format: yaml
  label: Marriott Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott-international/refs/heads/main/openapi/marriott-international-developer-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Marriott International Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Marriott International publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Marriott International API on a user''s behalf.


  Tokens are issued from https://devportalprod.marriott.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Marriott International
provider_slug: marriott-international
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://devportalprod.marriott.com/oauth/token
  name: oauth2
  source: openapi/marriott-international-developer-api-openapi.yml
scope_count: 2
scope_names:
- properties:read
- reservations:write
scopes:
- description: Read property information
  flows:
  - clientCredentials
  scope: properties:read
- description: Create and manage reservations
  flows:
  - clientCredentials
  scope: reservations:write
slug: marriott-international-scopes
source_filename: marriott-international-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marriott-international-developer-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/marriott-international-developer-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://devportalprod.marriott.com/oauth/token\nscopes:\n- scope: properties:read\n  description: Read property information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/marriott-international-developer-api-openapi.yml\n- scope: reservations:write\n  description: Create and manage reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/marriott-international-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott-international/refs/heads/main/scopes/marriott-international-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Fortune 500
token_urls:
- https://devportalprod.marriott.com/oauth/token
---
