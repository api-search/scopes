---
api_specs:
- filename: urbanfox-customer-api-openapi.yml
  format: yaml
  label: UrbanFox Customer API
  slug: urbanfox-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/openapi/urbanfox-customer-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.urbanfox.io/explanation/authentication-model
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Urbanfox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UrbanFox publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the UrbanFox API on a user''s behalf.


  Tokens are issued from https://api.demo-retail.urbanfox.io/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UrbanFox
provider_slug: urbanfox
schemes:
- description: 'OAuth 2.0 client-credentials flow. Request a token from `POST /v2/oauth/token` and send it as `Authorization: Bearer <access_token>`.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.demo-retail.urbanfox.io/v2/oauth/token
  name: oauth2
  source: openapi/urbanfox-customer-api-openapi.yml
scope_count: 13
scope_names:
- create:enduseraccount
- delete:enduseraccount
- read:case
- read:cases
- read:enduseraccount
- read:enduseraccounts
- read:metrics
- read:snippet
- read:tenant
- read:tenant_auth_secret
- update:case
- update:enduseraccount
- update:tenant_auth_secret
scopes:
- description: Create an end-user account
  flows:
  - clientCredentials
  scope: create:enduseraccount
- description: Delete an end-user account
  flows:
  - clientCredentials
  scope: delete:enduseraccount
- description: Get a case
  flows:
  - clientCredentials
  scope: read:case
- description: List cases
  flows:
  - clientCredentials
  scope: read:cases
- description: Get an end-user account
  flows:
  - clientCredentials
  scope: read:enduseraccount
- description: List end-user accounts
  flows:
  - clientCredentials
  scope: read:enduseraccounts
- description: Get tenant metrics
  flows:
  - clientCredentials
  scope: read:metrics
- description: Get integration snippets
  flows:
  - clientCredentials
  scope: read:snippet
- description: Get tenant
  flows:
  - clientCredentials
  scope: read:tenant
- description: Get tenant OAuth client credentials
  flows:
  - clientCredentials
  scope: read:tenant_auth_secret
- description: Update a case
  flows:
  - clientCredentials
  scope: update:case
- description: Update an end-user account
  flows:
  - clientCredentials
  scope: update:enduseraccount
- description: Rotate tenant OAuth client secret
  flows:
  - clientCredentials
  scope: update:tenant_auth_secret
slug: urbanfox-scopes
source_filename: urbanfox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/urbanfox-customer-api-openapi.yml\ndocs: https://docs.urbanfox.io/explanation/authentication-model\nnotes: 'Scopes follow the pattern action:resource and are additive; each protected\n  operation declares its required scope in its OAuth 2.0 security requirement, and\n  tokens missing the required scope receive a 403. Tokens are tenant-bound: a token\n  for one tenant slug cannot read or modify another tenant''s data.'\nschemes:\n- name: oauth2\n  source: openapi/urbanfox-customer-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.demo-retail.urbanfox.io/v2/oauth/token\n  description: 'OAuth 2.0 client-credentials flow. Request a token from `POST /v2/oauth/token`\n    and send it as `Authorization: Bearer <access_token>`.'\nscopes:\n- scope: create:enduseraccount\n  description: Create an end-user account\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n\
  - scope: delete:enduseraccount\n  description: Delete an end-user account\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:case\n  description: Get a case\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:cases\n  description: List cases\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:enduseraccount\n  description: Get an end-user account\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:enduseraccounts\n  description: List end-user accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:metrics\n  description: Get tenant metrics\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:snippet\n  description: Get integration snippets\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:tenant\n  description: Get tenant\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: read:tenant_auth_secret\n  description: Get tenant OAuth client credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: update:case\n  description: Update a case\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: update:enduseraccount\n  description: Update an end-user account\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n- scope: update:tenant_auth_secret\n  description: Rotate tenant OAuth client secret\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/urbanfox-customer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/scopes/urbanfox-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Fraud Detection
- Payment Fraud
- Account Takeover
- Bot Detection
- Risk Management
- Security
- Artificial Intelligence
- eCommerce
token_urls:
- https://api.demo-retail.urbanfox.io/v2/oauth/token
---
