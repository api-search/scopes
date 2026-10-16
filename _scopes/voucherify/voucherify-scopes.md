---
api_specs:
- filename: voucherify-openapi-generated.yml
  format: yaml
  label: Voucherify API
  slug: voucherify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/openapi/_ae-authored/voucherify-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Voucherify Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Voucherify publishes 42 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Voucherify API on a user''s behalf.


  Tokens are issued from https://{cluster}.voucherify.io/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Voucherify
provider_slug: voucherify
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{cluster}.voucherify.io/v1/oauth/token
  name: OAuth_2.0
  source: openapi/voucherify-openapi-generated.yml
scope_count: 42
scope_names:
- api
- assets
- async-actions
- campaigns
- categories
- client_api
- client_consents
- client_customers
- client_events
- client_promotions
- client_publish
- client_qualifications
- client_redeem
- client_redemptions
- client_validate
- client_validations
- client_vouchers
- consents
- customers
- events
- exports
- locations
- loyalties
- metadata-schemas
- orders
- product-collections
- products
- promotions
- publications
- qualifications
- redemptions
- referrals
- rewards
- segments
- skus
- task-results
- templates
- trash-bin
- validation-rules
- validation-rules-assignments
- validations
- vouchers
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: api
- description: ''
  flows:
  - clientCredentials
  scope: assets
- description: ''
  flows:
  - clientCredentials
  scope: async-actions
- description: ''
  flows:
  - clientCredentials
  scope: campaigns
- description: ''
  flows:
  - clientCredentials
  scope: categories
- description: ''
  flows:
  - clientCredentials
  scope: client_api
- description: ''
  flows:
  - clientCredentials
  scope: client_consents
- description: ''
  flows:
  - clientCredentials
  scope: client_customers
- description: ''
  flows:
  - clientCredentials
  scope: client_events
- description: ''
  flows:
  - clientCredentials
  scope: client_promotions
- description: ''
  flows:
  - clientCredentials
  scope: client_publish
- description: ''
  flows:
  - clientCredentials
  scope: client_qualifications
- description: ''
  flows:
  - clientCredentials
  scope: client_redeem
- description: ''
  flows:
  - clientCredentials
  scope: client_redemptions
- description: ''
  flows:
  - clientCredentials
  scope: client_validate
- description: ''
  flows:
  - clientCredentials
  scope: client_validations
- description: ''
  flows:
  - clientCredentials
  scope: client_vouchers
- description: ''
  flows:
  - clientCredentials
  scope: consents
- description: ''
  flows:
  - clientCredentials
  scope: customers
- description: ''
  flows:
  - clientCredentials
  scope: events
- description: ''
  flows:
  - clientCredentials
  scope: exports
- description: ''
  flows:
  - clientCredentials
  scope: locations
- description: ''
  flows:
  - clientCredentials
  scope: loyalties
- description: ''
  flows:
  - clientCredentials
  scope: metadata-schemas
- description: ''
  flows:
  - clientCredentials
  scope: orders
- description: ''
  flows:
  - clientCredentials
  scope: product-collections
- description: ''
  flows:
  - clientCredentials
  scope: products
- description: ''
  flows:
  - clientCredentials
  scope: promotions
- description: ''
  flows:
  - clientCredentials
  scope: publications
- description: ''
  flows:
  - clientCredentials
  scope: qualifications
- description: ''
  flows:
  - clientCredentials
  scope: redemptions
- description: ''
  flows:
  - clientCredentials
  scope: referrals
- description: ''
  flows:
  - clientCredentials
  scope: rewards
- description: ''
  flows:
  - clientCredentials
  scope: segments
- description: ''
  flows:
  - clientCredentials
  scope: skus
- description: ''
  flows:
  - clientCredentials
  scope: task-results
- description: ''
  flows:
  - clientCredentials
  scope: templates
- description: ''
  flows:
  - clientCredentials
  scope: trash-bin
- description: ''
  flows:
  - clientCredentials
  scope: validation-rules
- description: ''
  flows:
  - clientCredentials
  scope: validation-rules-assignments
- description: ''
  flows:
  - clientCredentials
  scope: validations
- description: ''
  flows:
  - clientCredentials
  scope: vouchers
slug: voucherify-scopes
source_filename: voucherify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/voucherify-openapi-generated.yml\nschemes:\n- name: OAuth_2.0\n  source: openapi/voucherify-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{cluster}.voucherify.io/v1/oauth/token\nscopes:\n- scope: api\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: assets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: async-actions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: campaigns\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: categories\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_api\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_consents\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_promotions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_publish\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_qualifications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_redeem\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_redemptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_validate\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n\
  - scope: client_validations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: client_vouchers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: consents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: exports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: locations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: loyalties\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: metadata-schemas\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n\
  - scope: orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: product-collections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: products\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: promotions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: publications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: qualifications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: redemptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: referrals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: rewards\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n\
  - scope: segments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: skus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: task-results\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: trash-bin\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: validation-rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: validation-rules-assignments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: validations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n- scope: vouchers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/voucherify-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/scopes/voucherify-scopes.yml
summary_line: 42 scopes · clientCredentials
tags:
- Company
- Incentives
- Promotions
- Loyalty
- API
token_bound: false
token_urls:
- https://{cluster}.voucherify.io/v1/oauth/token
---
