---
api_specs:
- filename: afterpay-openapi-generated.yml
  format: yaml
  label: Afterpay API
  slug: afterpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afterpay/refs/heads/main/openapi/_ae-authored/afterpay-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://developers.afterpay.com/afterpay-online-developer/main/guides/api-development/additional-features/account-linking-oauth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Afterpay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Afterpay publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Afterpay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Afterpay
provider_slug: afterpay
schemes: []
scope_count: 4
scope_names:
- merchant_api_v2
- merchant_api_v1
- read_user_info
- create_checkout
scopes:
- description: Client-credentials scope for the v2 merchant (Online) APIs.
  flows: []
  scope: merchant_api_v2
- description: Client-credentials scope to access the first version of the merchant APIs.
  flows: []
  scope: merchant_api_v1
- description: Permits access to the /oauth/v1/userinfo endpoint
  flows: []
  scope: read_user_info
- description: Allows the grant holder to create a checkout on behalf of the customer
  flows: []
  scope: create_checkout
slug: afterpay-scopes
source_filename: afterpay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Afterpay OAuth scopes\nprovider: afterpay\ngenerated: '2026-10-21'\nmethod: searched\nsource: https://developers.afterpay.com/afterpay-online-developer/main/guides/api-development/additional-features/account-linking-oauth.md\ndocs: https://developers.afterpay.com/afterpay-online-developer/main/guides/api-development/additional-features/account-linking-oauth\nscopes:\n- name: merchant_api_v2\n  description: Client-credentials scope for the v2 merchant (Online) APIs.\n  flow: clientCredentials\n  source: https://developers.afterpay.com/afterpay-online-developer/main/api-reference/reference/introduction/authentication\n- name: merchant_api_v1\n  description: Client-credentials scope to access the first version of the merchant APIs.\n  flow: clientCredentials\n  source: https://developers.afterpay.com/afterpay-online-developer/main/api-reference/reference/introduction/authentication\n- name: read_user_info\n  description: Permits access to the /oauth/v1/userinfo endpoint\n\
  \  flow: authorizationCode\n- name: create_checkout\n  description: Allows the grant holder to create a checkout on behalf of the customer\n  flow: authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterpay/refs/heads/main/scopes/afterpay-scopes.yml
summary_line: 4 scopes
tags:
- Fintech
- Buy Now Pay Later
- Payments
- Consumer
- Block
- Australia
- Consumer Finance
token_bound: false
token_urls: []
---
