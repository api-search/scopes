---
api_specs:
- filename: soldo-business-api-v20-openapi-original.json
  format: json
  label: Soldo Business API v2.0
  slug: soldo-business-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/openapi/soldo-business-api-v20-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Soldo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Soldo publishes 59 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Soldo API on a user''s behalf.


  Tokens are issued from https://api.soldo.com/oauth/authorize.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Soldo
provider_slug: soldo
schemes:
- description: This API uses OAuth 2 with the "Client Credentials" grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.soldo.com/oauth/authorize
  name: standardAuth
  source: openapi/soldo-business-api-v20-openapi-original.json
scope_count: 59
scope_names:
- address_read
- address_write
- autotag_read
- autotag_write
- business_trip_read
- business_trip_write
- card_read
- card_write
- company_read
- company_write
- contact_read
- contact_write
- document_read
- document_write
- employee_read
- employee_write
- expense_category_read
- expense_category_write
- expense_policy_read
- expense_policy_write
- expense_report_read
- expense_report_write
- expense_review_read
- expense_review_write
- group_read
- group_write
- online_ads_read
- online_ads_write
- order_read
- out_of_office_delegation_read
- out_of_office_delegation_write
- payment_read
- payment_write
- purchase_read
- purchase_write
- refueling_read
- refueling_write
- request_read
- request_write
- resource_set_read
- resource_set_write
- role_read
- statement_read
- subscription_read
- subscription_write
- tag_read
- tag_write
- tax_rate_read
- tax_rate_write
- transaction_read
- transaction_write
- vehicle_read
- vehicle_write
- wallet_read
- wallet_write
- webhook_subscription_read
- webhook_subscription_write
- workflow_read
- workflow_write
scopes:
- description: Can read address details.
  flows:
  - clientCredentials
  scope: address_read
- description: Can update address details.
  flows:
  - clientCredentials
  scope: address_write
- description: ''
  flows: []
  scope: autotag_read
- description: ''
  flows: []
  scope: autotag_write
- description: ''
  flows: []
  scope: business_trip_read
- description: ''
  flows: []
  scope: business_trip_write
- description: Can read card details.
  flows:
  - clientCredentials
  scope: card_read
- description: Can change card details.
  flows:
  - clientCredentials
  scope: card_write
- description: Can read company details.
  flows:
  - clientCredentials
  scope: company_read
- description: Can change company details.
  flows:
  - clientCredentials
  scope: company_write
- description: Can read contact details.
  flows:
  - clientCredentials
  scope: contact_read
- description: Can change contact details.
  flows:
  - clientCredentials
  scope: contact_write
- description: ''
  flows: []
  scope: document_read
- description: ''
  flows: []
  scope: document_write
- description: Can read employee details.
  flows:
  - clientCredentials
  scope: employee_read
- description: Can change employee details.
  flows:
  - clientCredentials
  scope: employee_write
- description: Can read expense category details.
  flows:
  - clientCredentials
  scope: expense_category_read
- description: Can change expense category details.
  flows:
  - clientCredentials
  scope: expense_category_write
- description: ''
  flows: []
  scope: expense_policy_read
- description: ''
  flows: []
  scope: expense_policy_write
- description: Can read expense report details.
  flows:
  - clientCredentials
  scope: expense_report_read
- description: Can change expense report details.
  flows:
  - clientCredentials
  scope: expense_report_write
- description: Can read expense review status.
  flows:
  - clientCredentials
  scope: expense_review_read
- description: Can change expense review status.
  flows:
  - clientCredentials
  scope: expense_review_write
- description: Can read group details.
  flows:
  - clientCredentials
  scope: group_read
- description: Can change groups details.
  flows:
  - clientCredentials
  scope: group_write
- description: Can read online ads details.
  flows:
  - clientCredentials
  scope: online_ads_read
- description: Can change online ads details.
  flows:
  - clientCredentials
  scope: online_ads_write
- description: ''
  flows: []
  scope: order_read
- description: ''
  flows: []
  scope: out_of_office_delegation_read
- description: ''
  flows: []
  scope: out_of_office_delegation_write
- description: Can read payment details.
  flows:
  - clientCredentials
  scope: payment_read
- description: Can change payment details.
  flows:
  - clientCredentials
  scope: payment_write
- description: Can read purchase details.
  flows:
  - clientCredentials
  scope: purchase_read
- description: Can change purchase details.
  flows:
  - clientCredentials
  scope: purchase_write
- description: Can read refueling details.
  flows:
  - clientCredentials
  scope: refueling_read
- description: Can change refueling details.
  flows:
  - clientCredentials
  scope: refueling_write
- description: ''
  flows: []
  scope: request_read
- description: ''
  flows: []
  scope: request_write
- description: Can read resource set details.
  flows:
  - clientCredentials
  scope: resource_set_read
- description: Can change resource set details.
  flows:
  - clientCredentials
  scope: resource_set_write
- description: Can read role details.
  flows:
  - clientCredentials
  scope: role_read
- description: Can read statement details.
  flows:
  - clientCredentials
  scope: statement_read
- description: Can read subscription details.
  flows:
  - clientCredentials
  scope: subscription_read
- description: Can change subscription details.
  flows:
  - clientCredentials
  scope: subscription_write
- description: Can read tags.
  flows:
  - clientCredentials
  scope: tag_read
- description: can change tags.
  flows:
  - clientCredentials
  scope: tag_write
- description: Can read vat rate details.
  flows:
  - clientCredentials
  scope: tax_rate_read
- description: Can change vat rate details.
  flows:
  - clientCredentials
  scope: tax_rate_write
- description: Can read transaction details.
  flows:
  - clientCredentials
  scope: transaction_read
- description: Can change transaction details.
  flows:
  - clientCredentials
  scope: transaction_write
- description: Can read vehicle details.
  flows:
  - clientCredentials
  scope: vehicle_read
- description: Can change vehicle details.
  flows:
  - clientCredentials
  scope: vehicle_write
- description: Can read wallet details.
  flows:
  - clientCredentials
  scope: wallet_read
- description: Can change wallet details.
  flows:
  - clientCredentials
  scope: wallet_write
- description: Can read webhook subscription details.
  flows:
  - clientCredentials
  scope: webhook_subscription_read
- description: Can change webhook subscription details.
  flows:
  - clientCredentials
  scope: webhook_subscription_write
- description: ''
  flows: []
  scope: workflow_read
- description: ''
  flows: []
  scope: workflow_write
slug: soldo-scopes
source_filename: soldo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soldo-business-api-v20-openapi-original.json\nschemes:\n- name: standardAuth\n  source: openapi/soldo-business-api-v20-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.soldo.com/oauth/authorize\n  description: This API uses OAuth 2 with the \"Client Credentials\" grant flow.\nscopes:\n- scope: address_read\n  description: Can read address details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: address_write\n  description: Can update address details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: autotag_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: autotag_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: business_trip_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n\
  - scope: business_trip_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: card_read\n  description: Can read card details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: card_write\n  description: Can change card details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: company_read\n  description: Can read company details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: company_write\n  description: Can change company details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: contact_read\n  description: Can read contact details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: contact_write\n  description: Can change contact details.\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: document_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: document_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: employee_read\n  description: Can read employee details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: employee_write\n  description: Can change employee details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_category_read\n  description: Can read expense category details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_category_write\n  description: Can change expense category details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n\
  - scope: expense_policy_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_policy_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_report_read\n  description: Can read expense report details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_report_write\n  description: Can change expense report details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_review_read\n  description: Can read expense review status.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: expense_review_write\n  description: Can change expense review status.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: group_read\n  description: Can read group details.\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: group_write\n  description: Can change groups details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: online_ads_read\n  description: Can read online ads details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: online_ads_write\n  description: Can change online ads details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: order_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: out_of_office_delegation_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: out_of_office_delegation_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: payment_read\n  description: Can read payment details.\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: payment_write\n  description: Can change payment details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: purchase_read\n  description: Can read purchase details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: purchase_write\n  description: Can change purchase details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: refueling_read\n  description: Can read refueling details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: refueling_write\n  description: Can change refueling details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: request_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n\
  - scope: request_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: resource_set_read\n  description: Can read resource set details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: resource_set_write\n  description: Can change resource set details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: role_read\n  description: Can read role details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: statement_read\n  description: Can read statement details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: subscription_read\n  description: Can read subscription details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: subscription_write\n  description:\
  \ Can change subscription details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: tag_read\n  description: Can read tags.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: tag_write\n  description: can change tags.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: tax_rate_read\n  description: Can read vat rate details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: tax_rate_write\n  description: Can change vat rate details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: transaction_read\n  description: Can read transaction details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: transaction_write\n  description:\
  \ Can change transaction details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: vehicle_read\n  description: Can read vehicle details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: vehicle_write\n  description: Can change vehicle details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: wallet_read\n  description: Can read wallet details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: wallet_write\n  description: Can change wallet details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: webhook_subscription_read\n  description: Can read webhook subscription details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n\
  - scope: webhook_subscription_write\n  description: Can change webhook subscription details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: workflow_read\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n- scope: workflow_write\n  sources:\n  - openapi/soldo-business-api-v20-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldo/refs/heads/main/scopes/soldo-scopes.yml
summary_line: 59 scopes · clientCredentials
tags:
- Company
- Consumer
- Fintech
- Financial Services
- Spend Management
- Expense Management
- Business Cards
- Prepaid Cards
- Payments
- Banking
token_urls:
- https://api.soldo.com/oauth/authorize
---
