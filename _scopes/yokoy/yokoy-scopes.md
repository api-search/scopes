---
api_specs:
- filename: yokoy-openapi-original.json
  format: json
  label: Yokoy API
  slug: yokoy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/openapi/yokoy-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Yokoy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yokoy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://accounts[.test].yokoy.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yokoy
provider_slug: yokoy
schemes:
- description: "Authentication to the Yokoy API relies on the standard OAuth2 client credentials flow.\n\n**1. Obtain an access token**\n\nPerform a `POST` request to\n`https://accounts.yokoy.ai/oauth2/token`. Pass the client ID\nand client secret as username and password in a basic auth\nheader. Set the content-type to\n`application/x-www-form-urlencoded` and specify\n`grant_type=client_credentials` in the body.\n\n> Note: For the Yokoy test environment, use `https://accounts.test.yokoy.ai/oauth2/token` instead.\n\nExample request for the client ID `ClientId` and client\nsecret `ClientSecret`:\n```\nPOST https://accounts.yokoy.ai/oauth2/token\nAuthorization: Basic Q2xpZW50SWQ6Q2xpZW50U2VjcmV0\nContent-Type: application/x-www-form-urlencoded\ngrant_type=client_credentials\n```\nIn this example, the string `Q2xpZW50SWQ6Q2xpZW50U2VjcmV0` is\nobtained by base64-encoding the string\n`ClientId:ClientSecret`, as required for basic access authentication.\n\n> Note: Yokoy does not require or use\
    \ scopes.\n\n\nThe JSON response contains the access token in the attribute\n`access_token`. The response also contains the expiration in\nseconds.\n\nExample response:\n```\n{\n    \"access_token\": \"SOME_KEY\",\n    \"expires_in\": 3900,\n    \"token_type\": \"Bearer\"\n}\n```\n\n**2. Pass the bearer token**\n\nPass the access token from step 1 as a bearer token in subsequent requests to the API.\n\nExample header field for the example response from step 1:\n```\nAuthorization: Bearer 4lDvPkrBF87WHuyvlINQD\n```\n\nFor more information, see (Authentication & authorization)[https://developer.yokoy.ai/docs/overview/authentication]."
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts[.test].yokoy.ai/oauth2/token
  name: OAuth2
  source: openapi/yokoy-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: yokoy-scopes
source_filename: yokoy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/yokoy-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/yokoy-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts[.test].yokoy.ai/oauth2/token\n  description: |-\n    Authentication to the Yokoy API relies on the standard OAuth2 client credentials flow.\n\n    **1. Obtain an access token**\n\n    Perform a `POST` request to\n    `https://accounts.yokoy.ai/oauth2/token`. Pass the client ID\n    and client secret as username and password in a basic auth\n    header. Set the content-type to\n    `application/x-www-form-urlencoded` and specify\n    `grant_type=client_credentials` in the body.\n\n    > Note: For the Yokoy test environment, use `https://accounts.test.yokoy.ai/oauth2/token` instead.\n\n    Example request for the client ID `ClientId` and client\n    secret `ClientSecret`:\n    ```\n    POST https://accounts.yokoy.ai/oauth2/token\n    Authorization: Basic\
  \ Q2xpZW50SWQ6Q2xpZW50U2VjcmV0\n    Content-Type: application/x-www-form-urlencoded\n    grant_type=client_credentials\n    ```\n    In this example, the string `Q2xpZW50SWQ6Q2xpZW50U2VjcmV0` is\n    obtained by base64-encoding the string\n    `ClientId:ClientSecret`, as required for basic access authentication.\n\n    > Note: Yokoy does not require or use scopes.\n\n\n    The JSON response contains the access token in the attribute\n    `access_token`. The response also contains the expiration in\n    seconds.\n\n    Example response:\n    ```\n    {\n        \"access_token\": \"SOME_KEY\",\n        \"expires_in\": 3900,\n        \"token_type\": \"Bearer\"\n    }\n    ```\n\n    **2. Pass the bearer token**\n\n    Pass the access token from step 1 as a bearer token in subsequent requests to the API.\n\n    Example header field for the example response from step 1:\n    ```\n    Authorization: Bearer 4lDvPkrBF87WHuyvlINQD\n    ```\n\n    For more information, see (Authentication & authorization)[https://developer.yokoy.ai/docs/overview/authentication].\n\
  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/scopes/yokoy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Spend Management
- Expense Management
- Invoice Management
- Finance Automation
- Corporate Cards
- Fintech
- SaaS
token_urls:
- https://accounts[.test].yokoy.ai/oauth2/token
---
