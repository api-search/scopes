---
api_specs:
- filename: kard-attributions-api-openapi.yml
  format: yaml
  label: Kard attributions API
  slug: kard-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-attributions-api-openapi.yml
- filename: kard-files-api-openapi.yml
  format: yaml
  label: Kard Files API
  slug: kard-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-files-api-openapi.yml
- filename: kard-notifications-notifications-api-openapi.yml
  format: yaml
  label: Kard notifications > Notifications API
  slug: kard-notifications-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-notifications-api-openapi.yml
- filename: kard-notifications-subscriptions-api-openapi.yml
  format: yaml
  label: Kard notifications > Subscriptions API
  slug: kard-notifications-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-subscriptions-api-openapi.yml
- filename: kard-organizations-api-openapi.yml
  format: yaml
  label: Kard Organizations API
  slug: kard-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-api-openapi.yml
- filename: kard-organizations-children-api-openapi.yml
  format: yaml
  label: Kard Organizations > Children API
  slug: kard-organizations-children-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-children-api-openapi.yml
- filename: kard-organizations-contentstrategies-api-openapi.yml
  format: yaml
  label: Kard Organizations > ContentStrategies API
  slug: kard-organizations-contentstrategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-contentstrategies-api-openapi.yml
- filename: kard-organizations-placements-api-openapi.yml
  format: yaml
  label: Kard Organizations > Placements API
  slug: kard-organizations-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-placements-api-openapi.yml
- filename: kard-ping-api-openapi.yml
  format: yaml
  label: Kard Ping API
  slug: kard-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-ping-api-openapi.yml
- filename: kard-rewards-api-openapi.yml
  format: yaml
  label: Kard rewards API
  slug: kard-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-rewards-api-openapi.yml
- filename: kard-transactions-api-openapi.yml
  format: yaml
  label: Kard transactions API
  slug: kard-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-transactions-api-openapi.yml
- filename: kard-users-api-openapi.yml
  format: yaml
  label: Kard users API
  slug: kard-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-api-openapi.yml
- filename: kard-users-attributions-api-openapi.yml
  format: yaml
  label: Kard users > attributions API
  slug: kard-users-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-attributions-api-openapi.yml
- filename: kard-users-rewards-api-openapi.yml
  format: yaml
  label: Kard users > Rewards API
  slug: kard-users-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-rewards-api-openapi.yml
- filename: kard-users-uploads-api-openapi.yml
  format: yaml
  label: Kard users > uploads API
  slug: kard-users-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-uploads-api-openapi.yml
- filename: kard-users-webview-api-openapi.yml
  format: yaml
  label: Kard users > WebView API
  slug: kard-users-webview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-webview-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.getkard.com/api/integration-guides/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kard Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kard publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kard API on a user''s behalf.


  Tokens are issued from https://{client-subdomain}.getkard.com/v2/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kard
provider_slug: kard
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{client-subdomain}.getkard.com/v2/auth/token
  name: OAuthScheme
  source: openapi/kard-api-reference-openapi.yaml
scope_count: 13
scope_names:
- transaction:read
- transaction:write
- audit:read
- audit:write
- user:read
- user:write
- user:update
- user:delete
- rewards:read
- attributions:write
- notifications:read
- notifications:write
- files:write
scopes:
- description: Read transactions and matched/earned reward data.
  flows:
  - clientCredentials
  scope: transaction:read
- description: Submit incoming transactions for CLO matching.
  flows:
  - clientCredentials
  scope: transaction:write
- description: Read transaction audit records.
  flows:
  - clientCredentials
  scope: audit:read
- description: Create transaction audit records.
  flows:
  - clientCredentials
  scope: audit:write
- description: Read enrolled user records.
  flows:
  - clientCredentials
  scope: user:read
- description: Create enrolled users.
  flows:
  - clientCredentials
  scope: user:write
- description: Update enrolled user records.
  flows:
  - clientCredentials
  scope: user:update
- description: Delete enrolled user records.
  flows:
  - clientCredentials
  scope: user:delete
- description: Read offers and locations available to a user.
  flows:
  - clientCredentials
  scope: rewards:read
- description: Create attribution events, activate and boost offers, activate placement slots.
  flows:
  - clientCredentials
  scope: attributions:write
- description: List and read notification events and subscriptions.
  flows:
  - clientCredentials
  scope: notifications:read
- description: Create/update notification subscriptions and replay notifications.
  flows:
  - clientCredentials
  scope: notifications:write
- description: Create and upload files / bulk transaction uploads.
  flows:
  - clientCredentials
  scope: files:write
slug: kard-scopes
source_filename: kard-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kard-api-reference-openapi.yaml\ndocs: https://docs.getkard.com/api/integration-guides/authentication\nschemes:\n- name: OAuthScheme\n  source: openapi/kard-api-reference-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{client-subdomain}.getkard.com/v2/auth/token\nnotes: The OpenAPI declares an http/bearer scheme, but the docs and per-operation\n  'Required scopes' annotations show OAuth2 client_credentials with the scopes below.\n  Scopes harvested from the OpenAPI operation descriptions.\nscopes:\n- scope: transaction:read\n  description: Read transactions and matched/earned reward data.\n  flows:\n  - clientCredentials\n- scope: transaction:write\n  description: Submit incoming transactions for CLO matching.\n  flows:\n  - clientCredentials\n- scope: audit:read\n  description: Read transaction audit records.\n  flows:\n  - clientCredentials\n- scope: audit:write\n  description: Create transaction\
  \ audit records.\n  flows:\n  - clientCredentials\n- scope: user:read\n  description: Read enrolled user records.\n  flows:\n  - clientCredentials\n- scope: user:write\n  description: Create enrolled users.\n  flows:\n  - clientCredentials\n- scope: user:update\n  description: Update enrolled user records.\n  flows:\n  - clientCredentials\n- scope: user:delete\n  description: Delete enrolled user records.\n  flows:\n  - clientCredentials\n- scope: rewards:read\n  description: Read offers and locations available to a user.\n  flows:\n  - clientCredentials\n- scope: attributions:write\n  description: Create attribution events, activate and boost offers, activate placement\n    slots.\n  flows:\n  - clientCredentials\n- scope: notifications:read\n  description: List and read notification events and subscriptions.\n  flows:\n  - clientCredentials\n- scope: notifications:write\n  description: Create/update notification subscriptions and replay notifications.\n  flows:\n  - clientCredentials\n\
  - scope: files:write\n  description: Create and upload files / bulk transaction uploads.\n  flows:\n  - clientCredentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/scopes/kard-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Company
- Rewards
- Card-Linked Offers
- Loyalty
- Fintech
- Commerce Media
- Advertising
- Transaction
- Cashback
- Webhook
token_urls:
- https://{client-subdomain}.getkard.com/v2/auth/token
---
