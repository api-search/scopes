---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Huntington Bancshares Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Huntington Bancshares publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Huntington Bancshares API on a user''s behalf.


  Tokens are issued from https://api.huntington.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Huntington Bancshares
provider_slug: huntington-bancshares
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.huntington.com/oauth/token
  name: oauth2
  source: openapi/huntington-bank-treasury-management-api-openapi.yml
scope_count: 3
scope_names:
- accounts:read
- payments:write
- transactions:read
scopes:
- description: Read account data
  flows:
  - clientCredentials
  scope: accounts:read
- description: Initiate payments
  flows:
  - clientCredentials
  scope: payments:write
- description: Read transactions
  flows:
  - clientCredentials
  scope: transactions:read
slug: huntington-bancshares-scopes
source_filename: huntington-bancshares-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/huntington-bank-treasury-management-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/huntington-bank-treasury-management-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.huntington.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/huntington-bank-treasury-management-api-openapi.yml\n- scope: payments:write\n  description: Initiate payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/huntington-bank-treasury-management-api-openapi.yml\n- scope: transactions:read\n  description: Read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/huntington-bank-treasury-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntington-bancshares/refs/heads/main/scopes/huntington-bancshares-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Banking
- ERP Integration
- Open Banking
- Payments
- Treasury
- Fortune 1000
token_urls:
- https://api.huntington.com/oauth/token
---
