---
authorization_urls:
- https://oauth.loopreturns.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Loop Returns Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Loop Returns publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Loop Returns API on a user''s behalf.


  Tokens are issued from https://oauth.loopreturns.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Loop Returns
provider_slug: loop-returns
schemes:
- flows:
  - authorizationUrl: https://oauth.loopreturns.com/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.loopreturns.com/oauth/token
  name: oauth2
  source: openapi/loop-returns-labels-openapi.yml
- description: OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://oauth.loopreturns.com/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.loopreturns.com/oauth/token
  name: oauth2
  source: openapi/loop-returns-webhooks-openapi.yml
scope_count: 6
scope_names:
- developer_tools
- label_requests:read
- label_requests:write
- labels:read
- labels:write
- returns
scopes:
- description: Access to developer tools including webhooks
  flows:
  - authorizationCode
  scope: developer_tools
- description: Read access to label requests
  flows:
  - authorizationCode
  scope: label_requests:read
- description: Create and modify label requests
  flows:
  - authorizationCode
  scope: label_requests:write
- description: Read access to labels
  flows:
  - authorizationCode
  scope: labels:read
- description: Create and modify labels
  flows:
  - authorizationCode
  scope: labels:write
- description: Access to returns operations
  flows:
  - authorizationCode
  scope: returns
slug: loop-returns-scopes
source_filename: loop-returns-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loop-returns-labels-openapi.yml, openapi/loop-returns-webhooks-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/loop-returns-labels-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.loopreturns.com/authorize\n    tokenUrl: https://oauth.loopreturns.com/oauth/token\n- name: oauth2\n  source: openapi/loop-returns-webhooks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.loopreturns.com/authorize\n    tokenUrl: https://oauth.loopreturns.com/oauth/token\n  description: OAuth 2.0 authorization\nscopes:\n- scope: developer_tools\n  description: Access to developer tools including webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-webhooks-openapi.yml\n- scope: label_requests:read\n  description: Read access to label requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n\
  - scope: label_requests:write\n  description: Create and modify label requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n- scope: labels:read\n  description: Read access to labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n- scope: labels:write\n  description: Create and modify labels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n- scope: returns\n  description: Access to returns operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/loop-returns-labels-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop-returns/refs/heads/main/scopes/loop-returns-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Returns
- E-Commerce
- Exchanges
- Refunds
- Shipping
- Post-Purchase
- Shopify
- Fraud Prevention
- Retail
token_urls:
- https://oauth.loopreturns.com/oauth/token
---
