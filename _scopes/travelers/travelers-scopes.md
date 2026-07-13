---
api_specs:
- filename: travelers-openapi.yml
  format: yaml
  label: Travelers API
  slug: travelers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/openapi/travelers-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Travelers Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Travelers publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Travelers API on a user''s behalf.


  Tokens are issued from https://api.travelers.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Travelers
provider_slug: travelers
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.travelers.com/oauth/token
  name: OAuth2
  source: openapi/travelers-openapi.yml
scope_count: 5
scope_names:
- claims:read
- claims:write
- policies:read
- quotes:read
- quotes:write
scopes:
- description: Read claim data
  flows:
  - clientCredentials
  scope: claims:read
- description: Submit and update claims
  flows:
  - clientCredentials
  scope: claims:write
- description: Read policy data
  flows:
  - clientCredentials
  scope: policies:read
- description: Read quote data
  flows:
  - clientCredentials
  scope: quotes:read
- description: Request quotes
  flows:
  - clientCredentials
  scope: quotes:write
slug: travelers-scopes
source_filename: travelers-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travelers-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/travelers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.travelers.com/oauth/token\nscopes:\n- scope: claims:read\n  description: Read claim data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/travelers-openapi.yml\n- scope: claims:write\n  description: Submit and update claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/travelers-openapi.yml\n- scope: policies:read\n  description: Read policy data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/travelers-openapi.yml\n- scope: quotes:read\n  description: Read quote data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/travelers-openapi.yml\n- scope: quotes:write\n  description: Request quotes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/travelers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/scopes/travelers-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Insurance
- Property Casualty
- Commercial Insurance
- Claims
- Fintech
- Fortune 500
token_urls:
- https://api.travelers.com/oauth/token
---
