---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Expedia Group Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Expedia Group publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Expedia Group API on a user''s behalf.


  Tokens are issued from https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Expedia Group
provider_slug: expedia-group
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials
  name: orderPurchaseScreenAuth
  source: openapi/expedia-fraud-protection-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials
  name: orderPurchaseUpdateAuth
  source: openapi/expedia-fraud-protection-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://test.analytics.ean.com/template/v1/oauth/token
  name: oauth
  source: openapi/expedia-loyalty-openapi-original.yml
scope_count: 3
scope_names:
- demand-solutions.demand-api-wrappers-prod.all
- fraudandrisk.fraud.order-purchase-screen
- fraudandrisk.fraud.order-purchase-update
scopes:
- description: Access to all Demand API Wrappers
  flows:
  - clientCredentials
  scope: demand-solutions.demand-api-wrappers-prod.all
- description: Use Fraud Systems for screening orders
  flows:
  - clientCredentials
  scope: fraudandrisk.fraud.order-purchase-screen
- description: Use Fraud Systems for updating orders
  flows:
  - clientCredentials
  scope: fraudandrisk.fraud.order-purchase-update
slug: expedia-group-scopes
source_filename: expedia-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/expedia-fraud-protection-openapi-original.yml, openapi/expedia-loyalty-openapi-original.yml\nschemes:\n- name: orderPurchaseScreenAuth\n  source: openapi/expedia-fraud-protection-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials\n- name: orderPurchaseUpdateAuth\n  source: openapi/expedia-fraud-protection-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials\n- name: oauth\n  source: openapi/expedia-loyalty-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://test.analytics.ean.com/template/v1/oauth/token\nscopes:\n- scope: demand-solutions.demand-api-wrappers-prod.all\n  description: Access to all Demand API Wrappers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/expedia-loyalty-openapi-original.yml\n\
  - scope: fraudandrisk.fraud.order-purchase-screen\n  description: Use Fraud Systems for screening orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/expedia-fraud-protection-openapi-original.yml\n- scope: fraudandrisk.fraud.order-purchase-update\n  description: Use Fraud Systems for updating orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/expedia-fraud-protection-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/scopes/expedia-group-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
token_urls:
- https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials
- https://test.analytics.ean.com/template/v1/oauth/token
---
