---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Shell Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shell publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shell API on a user''s behalf.


  Tokens are issued from https://api.shell.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shell
provider_slug: shell
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.shell.com/oauth/token
  name: OAuth2
  source: openapi/shell-b2b-mobility-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.shell.com/oauth/token
  name: OAuth2
  source: openapi/shell-loyalty-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.shell.com/oauth/token
  name: OAuth2
  source: openapi/shell-lubricants-openapi.yml
scope_count: 9
scope_names:
- loyalty.accounts
- loyalty.catalogue
- loyalty.points
- lubricants.orders
- lubricants.products
- mobility.cards
- mobility.invoices
- mobility.sites
- mobility.transactions
scopes:
- description: Manage loyalty accounts
  flows:
  - clientCredentials
  scope: loyalty.accounts
- description: Browse rewards catalogue
  flows:
  - clientCredentials
  scope: loyalty.catalogue
- description: Access points data
  flows:
  - clientCredentials
  scope: loyalty.points
- description: Manage lubricants orders
  flows:
  - clientCredentials
  scope: lubricants.orders
- description: Access product catalogue
  flows:
  - clientCredentials
  scope: lubricants.products
- description: Manage fuel cards
  flows:
  - clientCredentials
  scope: mobility.cards
- description: Access invoice data
  flows:
  - clientCredentials
  scope: mobility.invoices
- description: Query site data
  flows:
  - clientCredentials
  scope: mobility.sites
- description: Access transaction data
  flows:
  - clientCredentials
  scope: mobility.transactions
slug: shell-scopes
source_filename: shell-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shell-b2b-mobility-openapi.yml, openapi/shell-loyalty-openapi.yml, openapi/shell-lubricants-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/shell-b2b-mobility-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/oauth/token\n- name: OAuth2\n  source: openapi/shell-loyalty-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/oauth/token\n- name: OAuth2\n  source: openapi/shell-lubricants-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/oauth/token\nscopes:\n- scope: loyalty.accounts\n  description: Manage loyalty accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-loyalty-openapi.yml\n- scope: loyalty.catalogue\n  description: Browse rewards catalogue\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-loyalty-openapi.yml\n- scope: loyalty.points\n  description: Access\
  \ points data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-loyalty-openapi.yml\n- scope: lubricants.orders\n  description: Manage lubricants orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-lubricants-openapi.yml\n- scope: lubricants.products\n  description: Access product catalogue\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-lubricants-openapi.yml\n- scope: mobility.cards\n  description: Manage fuel cards\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-b2b-mobility-openapi.yml\n- scope: mobility.invoices\n  description: Access invoice data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-b2b-mobility-openapi.yml\n- scope: mobility.sites\n  description: Query site data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-b2b-mobility-openapi.yml\n- scope: mobility.transactions\n  description: Access transaction data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/shell-b2b-mobility-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/scopes/shell-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Aviation
- Electric Vehicle Charging
- Energy
- Fleet Management
- Fuel
- Gas
- Loyalty
- Lubricants
- Mobility
- Oil and Gas
- Renewable Energy
token_urls:
- https://api.shell.com/oauth/token
---
