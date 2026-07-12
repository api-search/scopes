---
authorization_urls:
- /v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bolt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bolt publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bolt API on a user''s behalf.


  Tokens are issued from /v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bolt
provider_slug: bolt
schemes:
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: /v1/oauth/token
  name: oauth
  source: openapi/bolt-api-reference-openapi.yaml
scope_count: 3
scope_names:
- bolt.account.manage
- bolt.account.view
- openid
scopes:
- description: This scope grants permissions to perform read/edit/delete actions on Bolt Account data
  flows:
  - authorizationCode
  scope: bolt.account.manage
- description: This scope grants permissions to perform read only actions on Bolt Account data
  flows:
  - authorizationCode
  scope: bolt.account.view
- description: This scope grants permissions that enable Bolt Single Sign-On (SSO) by granting a JSON Web Token (JWT) that stores account data.
  flows:
  - authorizationCode
  scope: openid
slug: bolt-scopes
source_filename: bolt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bolt-api-reference-openapi.yaml\nschemes:\n- name: oauth\n  source: openapi/bolt-api-reference-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\nscopes:\n- scope: bolt.account.manage\n  description: This scope grants permissions to perform read/edit/delete actions on Bolt Account\n    data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-api-reference-openapi.yaml\n- scope: bolt.account.view\n  description: This scope grants permissions to perform read only actions on Bolt Account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-api-reference-openapi.yaml\n- scope: openid\n  description: This scope grants permissions that enable Bolt Single Sign-On (SSO) by granting\n    a JSON Web Token (JWT) that stores account data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-api-reference-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt/refs/heads/main/scopes/bolt-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Checkout
- Payments
- eCommerce
- One-Click Checkout
- Shopper Network
- Fraud Protection
token_urls:
- /v1/oauth/token
---
