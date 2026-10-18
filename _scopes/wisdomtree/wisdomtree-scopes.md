---
api_specs:
- filename: wisdomtree-accruals-api-openapi.yml
  format: yaml
  label: WisdomTree Accruals API
  slug: wisdomtree-accruals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-accruals-api-openapi.yml
- filename: wisdomtree-dividend-payment-preferences-api-openapi.yml
  format: yaml
  label: WisdomTree Dividend Payment Preferences API
  slug: wisdomtree-dividend-payment-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-dividend-payment-preferences-api-openapi.yml
- filename: wisdomtree-fund-data-api-openapi.yml
  format: yaml
  label: WisdomTree Fund Data API
  slug: wisdomtree-fund-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-fund-data-api-openapi.yml
- filename: wisdomtree-orders-api-openapi.yml
  format: yaml
  label: WisdomTree Orders API
  slug: wisdomtree-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-orders-api-openapi.yml
- filename: wisdomtree-organizations-api-openapi.yml
  format: yaml
  label: WisdomTree Organizations API
  slug: wisdomtree-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-organizations-api-openapi.yml
- filename: wisdomtree-statements-api-openapi.yml
  format: yaml
  label: WisdomTree Statements API
  slug: wisdomtree-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-statements-api-openapi.yml
- filename: wisdomtree-users-api-openapi.yml
  format: yaml
  label: WisdomTree Users API
  slug: wisdomtree-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-users-api-openapi.yml
- filename: wisdomtree-wallets-api-openapi.yml
  format: yaml
  label: WisdomTree Wallets API
  slug: wisdomtree-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-wallets-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Wisdomtree Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WisdomTree publishes 3 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the WisdomTree API on a user''s behalf.


  Tokens are issued from https://app.wisdomtreeconnect.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WisdomTree
provider_slug: wisdomtree
schemes:
- flows:
  - flow: password
    tokenUrl: https://app.wisdomtreeconnect.com/o/token/
  name: oauth2
  source: openapi/wisdomtree-connect-openapi.yml
scope_count: 3
scope_names:
- groups
- read
- write
scopes:
- description: Access to your groups
  flows:
  - password
  scope: groups
- description: Read scope
  flows:
  - password
  scope: read
- description: Write scope
  flows:
  - password
  scope: write
slug: wisdomtree-scopes
source_filename: wisdomtree-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/wisdomtree-connect-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wisdomtree-connect-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://app.wisdomtreeconnect.com/o/token/\nscopes:\n- scope: groups\n  description: Access to your groups\n  flows:\n  - password\n  sources:\n  - openapi/wisdomtree-connect-openapi.yml\n- scope: read\n  description: Read scope\n  flows:\n  - password\n  sources:\n  - openapi/wisdomtree-connect-openapi.yml\n- scope: write\n  description: Write scope\n  flows:\n  - password\n  sources:\n  - openapi/wisdomtree-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/scopes/wisdomtree-scopes.yml
summary_line: 3 scopes · password
tags:
- Company
- Asset Management
- ETFs
- Tokenization
- Tokenized Funds
- Financial Services
- Fund Data
token_bound: false
token_urls:
- https://app.wisdomtreeconnect.com/o/token/
---
