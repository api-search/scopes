---
api_specs:
- filename: getpaid-accounts-api-openapi.yml
  format: yaml
  label: GetPaid Accounts API
  slug: getpaid-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-accounts-api-openapi.yml
- filename: getpaid-applications-api-openapi.yml
  format: yaml
  label: GetPaid Applications API
  slug: getpaid-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-applications-api-openapi.yml
- filename: getpaid-authentication-api-openapi.yml
  format: yaml
  label: GetPaid Authentication API
  slug: getpaid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-authentication-api-openapi.yml
- filename: getpaid-checkouts-api-openapi.yml
  format: yaml
  label: GetPaid Checkouts API
  slug: getpaid-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-checkouts-api-openapi.yml
- filename: getpaid-payments-api-openapi.yml
  format: yaml
  label: GetPaid Payments API
  slug: getpaid-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-payments-api-openapi.yml
- filename: getpaid-queries-api-openapi.yml
  format: yaml
  label: GetPaid Queries API
  slug: getpaid-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-queries-api-openapi.yml
- filename: getpaid-accept-payments-webhooks-api-openapi.yml
  format: yaml
  label: GetPaid Accept payments webhooks API
  slug: getpaid-accept-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-accept-payments-webhooks-api-openapi.yml
- filename: getpaid-onboard-sellers-webhooks-api-openapi.yml
  format: yaml
  label: GetPaid Onboard sellers webhooks API
  slug: getpaid-onboard-sellers-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-onboard-sellers-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Getpaid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GetPaid publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GetPaid API on a user''s behalf.


  Tokens are issued from https://auth.getpaid.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GetPaid
provider_slug: getpaid
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.getpaid.io/oauth/token
  name: OAuth
  source: openapi/getpaid-openapi-original.yml
scope_count: 4
scope_names:
- accounts:read
- accounts:read_write
- payments:read
- payments:read_write
scopes:
- description: Allows to read accounts and onboarding applications.
  flows:
  - clientCredentials
  scope: accounts:read
- description: Allows to read, create and/or operate accounts and onboarding applications.
  flows:
  - clientCredentials
  scope: accounts:read_write
- description: Allows to read payments and checkouts.
  flows:
  - clientCredentials
  scope: payments:read
- description: Allows to read, create and/or operate payments and checkouts.
  flows:
  - clientCredentials
  scope: payments:read_write
slug: getpaid-scopes
source_filename: getpaid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getpaid-openapi-original.yml\nschemes:\n- name: OAuth\n  source: openapi/getpaid-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.getpaid.io/oauth/token\nscopes:\n- scope: accounts:read\n  description: Allows to read accounts and onboarding applications.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getpaid-openapi-original.yml\n- scope: accounts:read_write\n  description: Allows to read, create and/or operate accounts and onboarding applications.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getpaid-openapi-original.yml\n- scope: payments:read\n  description: Allows to read payments and checkouts.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getpaid-openapi-original.yml\n- scope: payments:read_write\n  description: Allows to read, create and/or operate payments and checkouts.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/getpaid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/scopes/getpaid-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- Payments
- Embedded Payments
- Split Settlement
- Checkout
- Marketplace
- Onboarding
- Subscription
- Agent Payments
- Europe
token_urls:
- https://auth.getpaid.io/oauth/token
---
