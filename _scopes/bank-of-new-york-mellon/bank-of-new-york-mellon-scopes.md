---
api_specs:
- filename: bny-mellon-treasury-services-api-openapi.yml
  format: yaml
  label: BNY Mellon Treasury Services API
  slug: treasury-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/openapi/bny-mellon-treasury-services-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bank Of New York Mellon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BNY Mellon publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BNY Mellon API on a user''s behalf.


  Tokens are issued from https://api.bnymellon.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.bnymellon.com/oauth/token
  name: OAuth2
  source: openapi/bny-mellon-treasury-services-api-openapi.yml
scope_count: 5
scope_names:
- accounts:read
- balances:read
- payments:write
- transactions:read
- transfers:write
scopes:
- description: Read account data
  flows:
  - clientCredentials
  scope: accounts:read
- description: Read balance data
  flows:
  - clientCredentials
  scope: balances:read
- description: Initiate and manage payments
  flows:
  - clientCredentials
  scope: payments:write
- description: Read transaction history
  flows:
  - clientCredentials
  scope: transactions:read
- description: Initiate funds transfers
  flows:
  - clientCredentials
  scope: transfers:write
slug: bank-of-new-york-mellon-scopes
source_filename: bank-of-new-york-mellon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bny-mellon-treasury-services-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/bny-mellon-treasury-services-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.bnymellon.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n- scope: balances:read\n  description: Read balance data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n- scope: payments:write\n  description: Initiate and manage payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n- scope: transactions:read\n  description: Read transaction history\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n- scope: transfers:write\n\
  \  description: Initiate funds transfers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bny-mellon-treasury-services-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/scopes/bank-of-new-york-mellon-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
- Fortune 500
token_urls:
- https://api.bnymellon.com/oauth/token
---
