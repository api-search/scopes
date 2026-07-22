---
authorization_urls:
- https://toshl.com/oauth2/authorize
description: 'Toshl API OAuth 2.0 scopes. Scopes are granted per resource with :r (read) or :rw (read & write) access levels. The entries scope also grants access to tags, repeats, and export.

  '
docs: https://developer.toshl.com/docs/oauth
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Toshl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Toshl publishes 16 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Toshl API on a user''s behalf.


  Tokens are issued from https://toshl.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toshl
provider_slug: toshl
schemes:
- flows:
  - authorizationUrl: https://toshl.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://toshl.com/oauth2/token
  - authorizationUrl: https://toshl.com/oauth2/authorize
    flow: implicit
  name: OAuth2
  source: https://developer.toshl.com/docs/oauth
scope_count: 16
scope_names:
- user:r
- user:rw
- entries:r
- entries:rw
- budgets:r
- budgets:rw
- accounts:r
- accounts:rw
- images:r
- images:rw
- categories:r
- categories:rw
- tags:r
- tags:rw
- locations:r
- locations:rw
scopes:
- description: Read access to user information (email, name, etc.)
  flows: []
  scope: user:r
- description: Read and write access to user information
  flows: []
  scope: user:rw
- description: Read access to financial entries (expenses and incomes); also grants tags, repeats, and export access
  flows: []
  scope: entries:r
- description: Read and write access to financial entries; also grants tags, repeats, and export access
  flows: []
  scope: entries:rw
- description: Read access to budget data
  flows: []
  scope: budgets:r
- description: Read and write access to budget data
  flows: []
  scope: budgets:rw
- description: Read access to account information
  flows: []
  scope: accounts:r
- description: Read and write access to account information
  flows: []
  scope: accounts:rw
- description: Read access to entry images
  flows: []
  scope: images:r
- description: Read and write access to entry images (pro accounts only for upload)
  flows: []
  scope: images:rw
- description: Read access to spending categories
  flows: []
  scope: categories:r
- description: Read and write access to spending categories
  flows: []
  scope: categories:rw
- description: Read access to transaction tags
  flows: []
  scope: tags:r
- description: Read and write access to transaction tags
  flows: []
  scope: tags:rw
- description: Read access to entry locations
  flows: []
  scope: locations:r
- description: Read and write access to entry locations
  flows: []
  scope: locations:rw
slug: toshl-scopes
source_filename: toshl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.toshl.com/docs/oauth\ndocs: https://developer.toshl.com/docs/oauth\ndescription: >\n  Toshl API OAuth 2.0 scopes. Scopes are granted per resource with :r (read) or\n  :rw (read & write) access levels. The entries scope also grants access to\n  tags, repeats, and export.\nschemes:\n  - name: OAuth2\n    source: https://developer.toshl.com/docs/oauth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://toshl.com/oauth2/authorize\n        tokenUrl: https://toshl.com/oauth2/token\n      - flow: implicit\n        authorizationUrl: https://toshl.com/oauth2/authorize\nscopes:\n  - scope: user:r\n    description: Read access to user information (email, name, etc.)\n  - scope: user:rw\n    description: Read and write access to user information\n  - scope: entries:r\n    description: Read access to financial entries (expenses and incomes); also grants tags, repeats, and export access\n  -\
  \ scope: entries:rw\n    description: Read and write access to financial entries; also grants tags, repeats, and export access\n  - scope: budgets:r\n    description: Read access to budget data\n  - scope: budgets:rw\n    description: Read and write access to budget data\n  - scope: accounts:r\n    description: Read access to account information\n  - scope: accounts:rw\n    description: Read and write access to account information\n  - scope: images:r\n    description: Read access to entry images\n  - scope: images:rw\n    description: Read and write access to entry images (pro accounts only for upload)\n  - scope: categories:r\n    description: Read access to spending categories\n  - scope: categories:rw\n    description: Read and write access to spending categories\n  - scope: tags:r\n    description: Read access to transaction tags\n  - scope: tags:rw\n    description: Read and write access to transaction tags\n  - scope: locations:r\n    description: Read access to entry locations\n\
  \  - scope: locations:rw\n    description: Read and write access to entry locations\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toshl/refs/heads/main/scopes/toshl-scopes.yml
summary_line: 16 scopes · authorizationCode/implicit
tags:
- Personal Finance
- Budgeting
- Expense Tracking
- FinTech
- Banking
- Consumer Apps
- Company
token_urls:
- https://toshl.com/oauth2/token
---
