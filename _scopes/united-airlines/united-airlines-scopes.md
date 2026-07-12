---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: United Airlines Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'United Airlines publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the United Airlines API on a user''s behalf.


  Tokens are issued from https://api.united.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: United Airlines
provider_slug: united-airlines
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.united.com/v1/oauth/token
  name: OAuth2
  source: openapi/united-airlines-ndc-openapi.yml
scope_count: 2
scope_names:
- booking
- read
scopes:
- description: Full booking and servicing access
  flows:
  - clientCredentials
  scope: booking
- description: Read-only access to flight data
  flows:
  - clientCredentials
  scope: read
slug: united-airlines-scopes
source_filename: united-airlines-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-airlines-ndc-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/united-airlines-ndc-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.united.com/v1/oauth/token\nscopes:\n- scope: booking\n  description: Full booking and servicing access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/united-airlines-ndc-openapi.yml\n- scope: read\n  description: Read-only access to flight data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/united-airlines-ndc-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-airlines/refs/heads/main/scopes/united-airlines-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Airlines
- Travel
- Flight Booking
- NDC
- Loyalty
- Fortune 100
token_urls:
- https://api.united.com/v1/oauth/token
---
