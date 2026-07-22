---
api_specs:
- filename: teya-online-payments-openapi.yaml
  format: yaml
  label: Teya Online Payments API
  slug: teya-online-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-online-payments-openapi.yaml
- filename: teya-payments-openapi.yaml
  format: yaml
  label: Teya Payments Gateway API
  slug: teya-payments-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-payments-openapi.yaml
- filename: teya-poslink-openapi.json
  format: json
  label: Teya POSLink API
  slug: teya-poslink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-poslink-openapi.json
- filename: teya-fx-openapi.yaml
  format: yaml
  label: Teya FX (DCC) API
  slug: teya-fx-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-fx-openapi.yaml
authorization_urls:
- https://id.teya.xyz/oauth/v2/oauth-authorize
- https://id.teya.com/oauth/v2/oauth-authorize
description: ''
docs: https://docs.teya.com/apis/developer-portal/configure-application
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Teya Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Teya publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Teya API on a user''s behalf.


  Tokens are issued from https://id.teya.xyz/oauth/v2/oauth-token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Teya
provider_slug: teya
schemes:
- flows:
  - authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  - flow: clientCredentials
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  name: checkout_oauth_dev
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  - flow: clientCredentials
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: checkout_oauth_prd
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  - flow: clientCredentials
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: Ecommerce_Transaction_Payments_-_Public_oauth
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  - flow: clientCredentials
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  name: pbl_oauth_dev
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  - flow: clientCredentials
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: pbl_oauth_prd
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: Teya_Digital_Receipts_Service_oauth_prd
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: Payments_Refunds_Wrapper_API_oauth_prd
  source: openapi/teya-online-payments-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: oauth
  source: openapi/teya-payments-openapi.yaml
- description: 'Given a valid access token, you can now use a Bearer Token to authenticate your requests.

    To do so you have to preface your access token with Bearer and send it in the HTTP Authorization header.

    It should look something like this: `Authorization: Bearer <ACCESS_TOKEN>`'
  flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: authorisation
  source: openapi/teya-poslink-openapi.json
scope_count: 2
scope_names:
- terminal
- fx/dcc/create
scopes:
- description: Access to terminal/device payment and refund operations (client-credentials).
  flows:
  - clientCredentials
  scope: terminal
- description: Create Dynamic Currency Conversion (DCC) offers via the Teya FX API.
  flows:
  - authorizationCode
  scope: fx/dcc/create
slug: teya-scopes
source_filename: teya-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/teya-online-payments-openapi.yaml, openapi/teya-payments-openapi.yaml, openapi/teya-poslink-openapi.json\ndocs: https://docs.teya.com/apis/developer-portal/configure-application\nnotes: >-\n  OAuth applications are granted scopes in the Teya Developer Portal. The OpenAPI security\n  flows largely omit explicit scope maps; scopes below are those documented/observed\n  (terminal from the Payments Refunds Wrapper client-credentials flow, fx/dcc/create from the\n  DCC/FX API docs). Requesting a scope the application has not been granted returns 403.\nschemes:\n- name: checkout_oauth_dev\n  source: openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n- name: checkout_oauth_prd\n  source:\
  \ openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: Ecommerce_Transaction_Payments_-_Public_oauth\n  source: openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: pbl_oauth_dev\n  source: openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n- name: pbl_oauth_prd\n  source:\
  \ openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: Teya_Digital_Receipts_Service_oauth_prd\n  source: openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: Payments_Refunds_Wrapper_API_oauth_prd\n  source: openapi/teya-online-payments-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: oauth\n  source: openapi/teya-payments-openapi.yaml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n- name: authorisation\n  source: openapi/teya-poslink-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n  description: |-\n    Given a valid access token, you can now use a Bearer Token to authenticate your requests.\n    To do so you have to preface your access token with Bearer and send it in the HTTP Authorization header.\n    It should look something like this: `Authorization: Bearer <ACCESS_TOKEN>`\nscopes:\n- scope: terminal\n  description: Access to terminal/device payment and refund operations (client-credentials).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/teya-online-payments-openapi.yaml\n- scope: fx/dcc/create\n  description: Create\
  \ Dynamic Currency Conversion (DCC) offers via the Teya FX API.\n  flows:\n  - authorizationCode\n  sources:\n  - docs:https://docs.teya.com/apis/dynamic-currency-conversion/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/scopes/teya-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Payments
- Payment Processing
- Card Acquiring
- Online Payments
- Point of Sale
- E-commerce
- Fintech
- Merchant Services
- Europe
token_urls:
- https://id.teya.xyz/oauth/v2/oauth-token
- https://id.teya.com/oauth/v2/oauth-token
---
