---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SumUp REST API
  slug: sumup-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/sumup/sumup-openapi/main/openapi.yaml
authorization_urls:
- https://api.sumup.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sumup Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SumUp publishes 10 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SumUp API on a user''s behalf.


  Tokens are issued from https://api.sumup.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SumUp
provider_slug: sumup
schemes:
- description: 'SumUp supports [OAuth 2.0](https://tools.ietf.org/html/rfc6749) authentication for platforms that want to offer their services to SumUp users.


    To integrate via OAuth 2.0 you will need a client credentials that you can create in the [SumUp Dashboard](https://me.sumup.com/settings/oauth2-applications).


    To maintain security of our users, we highly recommend that you use one of the [recommended OAuth 2.0 libraries](https://oauth.net/code/) for authentication.'
  flows:
  - authorizationUrl: https://api.sumup.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.sumup.com/token
  - flow: clientCredentials
    tokenUrl: https://api.sumup.com/token
  name: oauth2
  source: openapi/openapi.yaml
scope_count: 10
scope_names:
- payment_instruments
- payments
- readers.read
- readers.write
- transactions.history
- user.app-settings
- user.payout-settings
- user.profile
- user.profile_readonly
- user.subaccounts
scopes:
- description: Manage customers and their payment instruments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payment_instruments
- description: Make payments by creating and processing checkouts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: ''
  flows: []
  scope: readers.read
- description: ''
  flows: []
  scope: readers.write
- description: View transactions and transaction history.
  flows:
  - authorizationCode
  - clientCredentials
  scope: transactions.history
- description: View and manage the SumUp mobile application settings.
  flows:
  - authorizationCode
  - clientCredentials
  scope: user.app-settings
- description: View and manage your payout settings.
  flows:
  - authorizationCode
  - clientCredentials
  scope: user.payout-settings
- description: View and manage your user profile.
  flows:
  - authorizationCode
  - clientCredentials
  scope: user.profile
- description: View user profile details.
  flows:
  - authorizationCode
  - clientCredentials
  scope: user.profile_readonly
- description: View and manage the user profile details of your employees.
  flows:
  - authorizationCode
  - clientCredentials
  scope: user.subaccounts
slug: sumup-scopes
source_filename: sumup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.sumup.com/authorize\n    tokenUrl: https://api.sumup.com/token\n  - flow: clientCredentials\n    tokenUrl: https://api.sumup.com/token\n  description: |-\n    SumUp supports [OAuth 2.0](https://tools.ietf.org/html/rfc6749) authentication for platforms that want to offer their services to SumUp users.\n\n    To integrate via OAuth 2.0 you will need a client credentials that you can create in the [SumUp Dashboard](https://me.sumup.com/settings/oauth2-applications).\n\n    To maintain security of our users, we highly recommend that you use one of the [recommended OAuth 2.0 libraries](https://oauth.net/code/) for authentication.\nscopes:\n- scope: payment_instruments\n  description: Manage customers and their payment instruments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/openapi.yaml\n- scope: payments\n  description: Make payments by creating and processing checkouts.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: readers.read\n  sources:\n  - openapi/openapi.yaml\n- scope: readers.write\n  sources:\n  - openapi/openapi.yaml\n- scope: transactions.history\n  description: View transactions and transaction history.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: user.app-settings\n  description: View and manage the SumUp mobile application settings.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: user.payout-settings\n  description: View and manage your payout settings.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: user.profile\n  description: View and manage your user profile.\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: user.profile_readonly\n  description: View user profile details.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n- scope: user.subaccounts\n  description: View and manage the user profile details of your employees.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/scopes/sumup-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials
tags:
- Payments
- POS
- Point of Sale
- Card Readers
- Checkout
- Fintech
- Mobile Payments
- Online Payments
token_urls:
- https://api.sumup.com/token
---
