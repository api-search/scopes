---
api_specs:
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Connect API
  slug: bud-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud First-Party Ingestion API
  slug: bud-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customers Platform API
  slug: bud-customers-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Data API
  slug: bud-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Enrichment API
  slug: bud-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Insights API
  slug: bud-financial-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Intelligent Search API
  slug: bud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Affordability and Assess API
  slug: bud-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customer Characteristics API
  slug: bud-characteristics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Goals and Budgets API
  slug: bud-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Payments API
  slug: bud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Embedded Widgets API
  slug: bud-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.thisisbud.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bud Co Scopes
name_suffix: OAuth Scopes
note: Bud's OAuth2 uses the client_credentials (and refresh_token) grant with API credentials granting full platform access; no OAuth scopes are used or documented (https://docs.thisisbud.com/docs/authentication).
overview: 'Bud Financial uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bud Financial
provider_slug: bud-co
schemes:
- description: "Authentication flow:\n\n1. Perform OAuth2 Client Credentials authentication using API Credentials (`client_id`,`client_secret`) to obtain an `access_token` against `/v1/oauth/token` endpoint,\n2. Use `access_token` as Bearer Authorisation for every other API request,\n3. Include `X-Client-Id` (=client_id) within the header of every API request,\n4. Note that some of the requests may also require `X-Customer-Id` to be provided within the request header.\n\n### Examples\nObtain OAuth2 `access_token` and `refresh_token` using `grant_type=client_credentials` and HTTP Basic auth header\n\n```\ncurl --basic --user {{client_id}}:{{client_secret}} \\\n  -X POST https://api-sandbox.thisisbud.com/v1/oauth/token \\\n  -H 'Content-Type: application/x-www-form-urlencoded' \\\n  -d grant_type=client_credentials\n```\n\nSuccessful response:\n```\n{\n  \"operation_id\": \"oauth_token_post\",\n  \"data\": {\n    \"access_token\": \"dd0c17e3fd6d2ce94aa091257a3ea393b4f9b5cf3d3e998f07dc9826da86ff15\"\
    ,\n    \"token_type\": \"bearer\",\n    \"expires_in\": 3600,\n    \"refresh_token\": \"fac32cca7559d9f6e8f1dfe9a99c71fa1dcfeb482bedf287d7934d2667ae54b3\"\n  }\n}\n```\n\nRefresh `access_token` token using `refresh_token` against `/v1/oauth/token` endpoint with `grant_type=refresh_token`\n\n```\ncurl -X POST \\\n  https://api-sandbox.thisisbud.com/v1/oauth/token \\\n  -H 'Content-Type: application/x-www-form-urlencoded' \\\n  -H 'X-Client-Id: {{client_id}}' \\\n  -d 'grant_type=refresh_token&refresh_token={{refresh_token}}'\n```\n\nSuccessful response:\n```\n{\n    \"operation_id\": \"oauth_token_post\",\n    \"data\": {\n        \"access_token\": \"cc0c17e3fd6d2ce94aa091257a3ea393b4f9b5cf3d3e998f07dc9826da86ff94\",\n        \"token_type\": \"bearer\",\n        \"expires_in\": 3600,\n        \"refresh_token\": \"ffc30cca7559d9f6e8f1dfe9a99c71fa1dcfeb482bedf287d7934d2667ae54b3\"\n    }\n}\n```"
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth/token
  name: OAuth2
  source: openapi/bud-platform-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: bud-co-scopes
source_filename: bud-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bud-platform-openapi.yml\ndocs: https://docs.thisisbud.com/docs/authentication\nnote: >-\n  Bud's OAuth2 uses the client_credentials (and refresh_token) grant with API\n  credentials granting full platform access; no OAuth scopes are used or\n  documented (https://docs.thisisbud.com/docs/authentication).\nschemes:\n- name: OAuth2\n  source: openapi/bud-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/token\n  description: |-\n    Authentication flow:\n\n    1. Perform OAuth2 Client Credentials authentication using API Credentials (`client_id`,`client_secret`) to obtain an `access_token` against `/v1/oauth/token` endpoint,\n    2. Use `access_token` as Bearer Authorisation for every other API request,\n    3. Include `X-Client-Id` (=client_id) within the header of every API request,\n    4. Note that some of the requests may also require `X-Customer-Id` to be provided within the request\
  \ header.\n\n    ### Examples\n    Obtain OAuth2 `access_token` and `refresh_token` using `grant_type=client_credentials` and HTTP Basic auth header\n\n    ```\n    curl --basic --user {{client_id}}:{{client_secret}} \\\n      -X POST https://api-sandbox.thisisbud.com/v1/oauth/token \\\n      -H 'Content-Type: application/x-www-form-urlencoded' \\\n      -d grant_type=client_credentials\n    ```\n\n    Successful response:\n    ```\n    {\n      \"operation_id\": \"oauth_token_post\",\n      \"data\": {\n        \"access_token\": \"dd0c17e3fd6d2ce94aa091257a3ea393b4f9b5cf3d3e998f07dc9826da86ff15\",\n        \"token_type\": \"bearer\",\n        \"expires_in\": 3600,\n        \"refresh_token\": \"fac32cca7559d9f6e8f1dfe9a99c71fa1dcfeb482bedf287d7934d2667ae54b3\"\n      }\n    }\n    ```\n\n    Refresh `access_token` token using `refresh_token` against `/v1/oauth/token` endpoint with `grant_type=refresh_token`\n\n    ```\n    curl -X POST \\\n      https://api-sandbox.thisisbud.com/v1/oauth/token\
  \ \\\n      -H 'Content-Type: application/x-www-form-urlencoded' \\\n      -H 'X-Client-Id: {{client_id}}' \\\n      -d 'grant_type=refresh_token&refresh_token={{refresh_token}}'\n    ```\n\n    Successful response:\n    ```\n    {\n        \"operation_id\": \"oauth_token_post\",\n        \"data\": {\n            \"access_token\": \"cc0c17e3fd6d2ce94aa091257a3ea393b4f9b5cf3d3e998f07dc9826da86ff94\",\n            \"token_type\": \"bearer\",\n            \"expires_in\": 3600,\n            \"refresh_token\": \"ffc30cca7559d9f6e8f1dfe9a99c71fa1dcfeb482bedf287d7934d2667ae54b3\"\n        }\n    }\n    ```\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/scopes/bud-co-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Open Banking
- Transaction Enrichment
- Categorization
- Affordability
- Payments
- AISP
- PISP
- Financial Data
- FinTech
- UK
- AI
- Machine Learning
token_urls:
- /v1/oauth/token
---
