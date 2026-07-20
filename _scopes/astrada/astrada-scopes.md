---
api_specs:
- filename: astrada-openapi-original.json
  format: json
  label: Astrada API
  slug: astrada-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-openapi-original.json
authorization_urls:
- https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Astrada Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Astrada publishes 34 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Astrada API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Astrada
provider_slug: astrada
schemes:
- flows:
  - authorizationUrl: https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token
    flow: implicit
  name: main-auth
  source: openapi/astrada-openapi-original.json
scope_count: 34
scope_names:
- accounts:read
- accounts:write
- appstore:cards:read
- appstore:enrollment:write
- appstore:sessions:read
- appstore:sessions:write
- appstore:tokens:read
- appstore:tokens:write
- appstore:transactions:read
- appstore:transactions:sync
- banking:admin
- banking:read
- banking:write
- card-connector-consents:read
- card-connector-consents:write
- card-connector-data-links:write
- card-subscriptions:read
- card-subscriptions:write
- card-verifications:read
- card-verifications:write
- cardholder:read
- cardholder:write
- cards:read
- enrollment-methods:write
- network-bulk-feeds:read
- network-bulk-feeds:write
- network-links:write
- simulation:write
- subaccounts:read
- subaccounts:write
- transaction-messages:read
- transactions:read
- webhooks:read
- webhooks:write
scopes:
- description: Accounts read resource
  flows:
  - implicit
  scope: accounts:read
- description: Accounts write resource
  flows:
  - implicit
  scope: accounts:write
- description: View enrolled cards in the appstore
  flows:
  - implicit
  scope: appstore:cards:read
- description: Enroll cards via the appstore B2C flow
  flows:
  - implicit
  scope: appstore:enrollment:write
- description: Read appstore session state
  flows:
  - implicit
  scope: appstore:sessions:read
- description: Write or delete appstore session state
  flows:
  - implicit
  scope: appstore:sessions:write
- description: Read appstore stored tokens and connections
  flows:
  - implicit
  scope: appstore:tokens:read
- description: Write appstore stored tokens and connections
  flows:
  - implicit
  scope: appstore:tokens:write
- description: View synced transactions in the appstore
  flows:
  - implicit
  scope: appstore:transactions:read
- description: Trigger transaction sync in the appstore
  flows:
  - implicit
  scope: appstore:transactions:sync
- description: Admin banking operations
  flows:
  - implicit
  scope: banking:admin
- description: Read banking resources
  flows:
  - implicit
  scope: banking:read
- description: Write banking resources
  flows:
  - implicit
  scope: banking:write
- description: Card Consent read resource
  flows:
  - implicit
  scope: card-connector-consents:read
- description: Card Consent write resource
  flows:
  - implicit
  scope: card-connector-consents:write
- description: card-connector-data-link resource
  flows:
  - implicit
  scope: card-connector-data-links:write
- description: Read card subscription
  flows:
  - implicit
  scope: card-subscriptions:read
- description: Create card subscription
  flows:
  - implicit
  scope: card-subscriptions:write
- description: Read Card verification
  flows:
  - implicit
  scope: card-verifications:read
- description: Create card verification
  flows:
  - implicit
  scope: card-verifications:write
- description: Read Cardholder resources
  flows:
  - implicit
  scope: cardholder:read
- description: Write Cardholder resources
  flows:
  - implicit
  scope: cardholder:write
- description: Read Card resources
  flows:
  - implicit
  scope: cards:read
- description: Write enrollment methods
  flows:
  - implicit
  scope: enrollment-methods:write
- description: Read network bulk feed
  flows:
  - implicit
  scope: network-bulk-feeds:read
- description: Write network bulk feed
  flows:
  - implicit
  scope: network-bulk-feeds:write
- description: Write network link
  flows:
  - implicit
  scope: network-links:write
- description: Write sandbox simulations
  flows:
  - implicit
  scope: simulation:write
- description: Subaccounts read resource
  flows:
  - implicit
  scope: subaccounts:read
- description: Subaccounts write resource
  flows:
  - implicit
  scope: subaccounts:write
- description: Read Transaction Message resources
  flows:
  - implicit
  scope: transaction-messages:read
- description: Read Transaction resources
  flows:
  - implicit
  scope: transactions:read
- description: Read Webhook resources
  flows:
  - implicit
  scope: webhooks:read
- description: Write Webhook resources
  flows:
  - implicit
  scope: webhooks:write
slug: astrada-scopes
source_filename: astrada-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/astrada-openapi-original.json\nschemes:\n- name: main-auth\n  source: openapi/astrada-openapi-original.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token\nscopes:\n- scope: accounts:read\n  description: Accounts read resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: accounts:write\n  description: Accounts write resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:cards:read\n  description: View enrolled cards in the appstore\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:enrollment:write\n  description: Enroll cards via the appstore B2C flow\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:sessions:read\n  description: Read appstore session\
  \ state\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:sessions:write\n  description: Write or delete appstore session state\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:tokens:read\n  description: Read appstore stored tokens and connections\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:tokens:write\n  description: Write appstore stored tokens and connections\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:transactions:read\n  description: View synced transactions in the appstore\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: appstore:transactions:sync\n  description: Trigger transaction sync in the appstore\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: banking:admin\n  description: Admin banking operations\n\
  \  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: banking:read\n  description: Read banking resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: banking:write\n  description: Write banking resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-connector-consents:read\n  description: Card Consent read resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-connector-consents:write\n  description: Card Consent write resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-connector-data-links:write\n  description: card-connector-data-link resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-subscriptions:read\n  description: Read card subscription\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n\
  - scope: card-subscriptions:write\n  description: Create card subscription\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-verifications:read\n  description: Read Card verification\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: card-verifications:write\n  description: Create card verification\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: cardholder:read\n  description: Read Cardholder resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: cardholder:write\n  description: Write Cardholder resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: cards:read\n  description: Read Card resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: enrollment-methods:write\n  description: Write enrollment methods\n  flows:\n  - implicit\n  sources:\n\
  \  - openapi/astrada-openapi-original.json\n- scope: network-bulk-feeds:read\n  description: Read network bulk feed\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: network-bulk-feeds:write\n  description: Write network bulk feed\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: network-links:write\n  description: Write network link\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: simulation:write\n  description: Write sandbox simulations\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: subaccounts:read\n  description: Subaccounts read resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: subaccounts:write\n  description: Subaccounts write resource\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: transaction-messages:read\n  description: Read Transaction\
  \ Message resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: transactions:read\n  description: Read Transaction resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: webhooks:read\n  description: Read Webhook resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n- scope: webhooks:write\n  description: Write Webhook resources\n  flows:\n  - implicit\n  sources:\n  - openapi/astrada-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/scopes/astrada-scopes.yml
summary_line: 34 scopes · implicit
tags:
- Company
- Fintech
- Payments
- Card Data
- Transaction Data
- Reconciliation
- Expense Management
- Data Infrastructure
token_urls: []
---
