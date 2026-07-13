---
api_specs:
- filename: upvest-investment-api-openapi.yml
  format: yaml
  label: Upvest Investment API
  slug: investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/openapi/upvest-investment-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Upvest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upvest publishes 18 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upvest API on a user''s behalf.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upvest
provider_slug: upvest
schemes:
- description: OAuth 2.0 client credentials flow. Obtain an access token by providing your client ID and client secret.
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2ClientCredentials
  source: openapi/upvest-investment-api-openapi.yml
scope_count: 18
scope_names:
- accounts:admin
- accounts:read
- fees:admin
- fees:read
- instruments:read
- orders:admin
- orders:read
- payments:admin
- payments:read
- portfolios:admin
- portfolios:read
- positions:read
- reports:read
- transactions:read
- users:admin
- users:read
- webhooks:admin
- webhooks:read
scopes:
- description: Create and manage accounts
  flows:
  - clientCredentials
  scope: accounts:admin
- description: Read account data
  flows:
  - clientCredentials
  scope: accounts:read
- description: Configure fees
  flows:
  - clientCredentials
  scope: fees:admin
- description: Read fee data
  flows:
  - clientCredentials
  scope: fees:read
- description: Read instrument data
  flows:
  - clientCredentials
  scope: instruments:read
- description: Place and manage orders
  flows:
  - clientCredentials
  scope: orders:admin
- description: Read order data
  flows:
  - clientCredentials
  scope: orders:read
- description: Manage payments and direct debits
  flows:
  - clientCredentials
  scope: payments:admin
- description: Read payment data
  flows:
  - clientCredentials
  scope: payments:read
- description: Create and manage portfolios
  flows:
  - clientCredentials
  scope: portfolios:admin
- description: Read portfolio data
  flows:
  - clientCredentials
  scope: portfolios:read
- description: Read position data
  flows:
  - clientCredentials
  scope: positions:read
- description: Read reports
  flows:
  - clientCredentials
  scope: reports:read
- description: Read transaction data
  flows:
  - clientCredentials
  scope: transactions:read
- description: Onboard and manage users
  flows:
  - clientCredentials
  scope: users:admin
- description: Read user data
  flows:
  - clientCredentials
  scope: users:read
- description: Manage webhook subscriptions
  flows:
  - clientCredentials
  scope: webhooks:admin
- description: Read webhook subscriptions
  flows:
  - clientCredentials
  scope: webhooks:read
slug: upvest-scopes
source_filename: upvest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upvest-investment-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/upvest-investment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials flow. Obtain an access token by providing your client\n    ID and client secret.\nscopes:\n- scope: accounts:admin\n  description: Create and manage accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: accounts:read\n  description: Read account data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: fees:admin\n  description: Configure fees\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: fees:read\n  description: Read fee data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n-\
  \ scope: instruments:read\n  description: Read instrument data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: orders:admin\n  description: Place and manage orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: orders:read\n  description: Read order data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: payments:admin\n  description: Manage payments and direct debits\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: payments:read\n  description: Read payment data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: portfolios:admin\n  description: Create and manage portfolios\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: portfolios:read\n  description: Read portfolio data\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: positions:read\n  description: Read position data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: reports:read\n  description: Read reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: transactions:read\n  description: Read transaction data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: users:admin\n  description: Onboard and manage users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: users:read\n  description: Read user data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n- scope: webhooks:admin\n  description: Manage webhook subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n\
  - scope: webhooks:read\n  description: Read webhook subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upvest-investment-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/scopes/upvest-scopes.yml
summary_line: 18 scopes · clientCredentials
tags:
- Banking Infrastructure
- Fintech
- Investments
- Securities
- Fractional Investing
- Custody
- Wealth Management
token_urls:
- /auth/token
---
