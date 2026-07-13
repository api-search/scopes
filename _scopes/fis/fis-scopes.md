---
api_specs:
- filename: fis-payments-openapi.yml
  format: yaml
  label: FIS Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Fis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FIS Global publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FIS Global API on a user''s behalf.


  Tokens are issued from https://api.fisglobal.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FIS Global
provider_slug: fis
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.fisglobal.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/fis-payments-openapi.yml
scope_count: 3
scope_names:
- accounts:read
- payments:read
- payments:write
scopes:
- description: Read account information
  flows:
  - clientCredentials
  scope: accounts:read
- description: Read payment data
  flows:
  - clientCredentials
  scope: payments:read
- description: Create and modify payments
  flows:
  - clientCredentials
  scope: payments:write
slug: fis-scopes
source_filename: fis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fis-payments-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/fis-payments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.fisglobal.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/fis-payments-openapi.yml\n- scope: payments:read\n  description: Read payment data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/fis-payments-openapi.yml\n- scope: payments:write\n  description: Create and modify payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/fis-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/scopes/fis-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Banking
- Core Banking
- Financial Services
- Payments
- Fintech
token_urls:
- https://api.fisglobal.com/oauth/token
---
