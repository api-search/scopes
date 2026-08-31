---
api_specs:
- filename: moneris-3d-secure-api-openapi.yml
  format: yaml
  label: Moneris 3D Secure API
  slug: moneris-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-3d-secure-api-openapi.yml
- filename: moneris-customers-api-openapi.yml
  format: yaml
  label: Moneris Customers API
  slug: moneris-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-customers-api-openapi.yml
- filename: moneris-disputes-api-openapi.yml
  format: yaml
  label: Moneris Disputes API
  slug: moneris-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-disputes-api-openapi.yml
- filename: moneris-installments-api-openapi.yml
  format: yaml
  label: Moneris Installments API
  slug: moneris-installments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-installments-api-openapi.yml
- filename: moneris-kount-api-openapi.yml
  format: yaml
  label: Moneris Kount API
  slug: moneris-kount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-kount-api-openapi.yml
- filename: moneris-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Moneris Merchant Onboarding API
  slug: moneris-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-merchant-onboarding-api-openapi.yml
- filename: moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
  format: yaml
  label: Moneris Multi-Currency Pricing Rate Lookup API
  slug: moneris-multi-currency-pricing-rate-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
- filename: moneris-payment-methods-api-openapi.yml
  format: yaml
  label: Moneris Payment Methods API
  slug: moneris-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payment-methods-api-openapi.yml
- filename: moneris-payments-api-openapi.yml
  format: yaml
  label: Moneris Payments API
  slug: moneris-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payments-api-openapi.yml
- filename: moneris-products-api-openapi.yml
  format: yaml
  label: Moneris Products API
  slug: moneris-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-products-api-openapi.yml
- filename: moneris-refunds-api-openapi.yml
  format: yaml
  label: Moneris Refunds API
  slug: moneris-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-refunds-api-openapi.yml
- filename: moneris-subscriptions-api-openapi.yml
  format: yaml
  label: Moneris Subscriptions API
  slug: moneris-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-subscriptions-api-openapi.yml
- filename: moneris-surcharge-lookup-api-openapi.yml
  format: yaml
  label: Moneris Surcharge Lookup API
  slug: moneris-surcharge-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-surcharge-lookup-api-openapi.yml
- filename: moneris-terminal-service-orders-api-openapi.yml
  format: yaml
  label: Moneris Terminal & Service Orders API
  slug: moneris-terminal-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-terminal-service-orders-api-openapi.yml
- filename: moneris-validations-api-openapi.yml
  format: yaml
  label: Moneris Validations API
  slug: moneris-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-validations-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Moneris Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moneris publishes 14 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Moneris API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moneris
provider_slug: moneris
schemes:
- description: 'OAuth 2.0 is an authorization protocol that gives an API client limited access to user data on a web server.


    OAuth relies on authentication scenarios, that allows the resource owner (user) to share the protected content from the server, hosting the resource, without sharing their credentials. For that purpose, an OAuth 2.0 server issues access tokens that the client applications can use to access protected resources on behalf of the resource owner.


    Moneris recommends the use of OAuth 2.0 as it provides fine grained authorization levels.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/moneris-unified-api-openapi.json
scope_count: 14
scope_names:
- customer.read
- customer.write
- dispute.read
- dispute.write
- kount.read
- kount.write
- onboarding.merchant.read
- onboarding.merchant.write
- onboarding.order.read
- onboarding.order.write
- payment.read
- payment.write
- refund.read
- refund.write
scopes:
- description: Grants read access to customer data
  flows:
  - clientCredentials
  scope: customer.read
- description: Grants read & write access to customer data
  flows:
  - clientCredentials
  scope: customer.write
- description: Grants read access to disputes
  flows:
  - clientCredentials
  scope: dispute.read
- description: Grants read & write access to disputes
  flows:
  - clientCredentials
  scope: dispute.write
- description: Grants read access to Kount inquiries
  flows:
  - clientCredentials
  scope: kount.read
- description: Grants read & write access to Kount inquiries
  flows:
  - clientCredentials
  scope: kount.write
- description: Grants read access to merchant onboarding related APIs
  flows:
  - clientCredentials
  scope: onboarding.merchant.read
- description: Grants read & write access to merchant onboarding related APIs
  flows:
  - clientCredentials
  scope: onboarding.merchant.write
- description: Grants read access to onboarding orders related APIs
  flows:
  - clientCredentials
  scope: onboarding.order.read
- description: Grants read & write access to onboarding orders related APIs
  flows:
  - clientCredentials
  scope: onboarding.order.write
- description: Grants read access to payment related APIs
  flows:
  - clientCredentials
  scope: payment.read
- description: Grants read & write access to payment related APIs
  flows:
  - clientCredentials
  scope: payment.write
- description: Grants read access to refunds
  flows:
  - clientCredentials
  scope: refund.read
- description: Grants read & write access to refunds
  flows:
  - clientCredentials
  scope: refund.write
slug: moneris-scopes
source_filename: moneris-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/moneris-unified-api-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/moneris-unified-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: |-\n    OAuth 2.0 is an authorization protocol that gives an API client limited access to user data on a web server.\n\n    OAuth relies on authentication scenarios, that allows the resource owner (user) to share the protected content from the server, hosting the resource, without sharing their credentials. For that purpose, an OAuth 2.0 server issues access tokens that the client applications can use to access protected resources on behalf of the resource owner.\n\n    Moneris recommends the use of OAuth 2.0 as it provides fine grained authorization levels.\nscopes:\n- scope: customer.read\n  description: Grants read access to customer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n\
  - scope: customer.write\n  description: Grants read & write access to customer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: dispute.read\n  description: Grants read access to disputes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: dispute.write\n  description: Grants read & write access to disputes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: kount.read\n  description: Grants read access to Kount inquiries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: kount.write\n  description: Grants read & write access to Kount inquiries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: onboarding.merchant.read\n  description: Grants read access to merchant onboarding related APIs\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/moneris-unified-api-openapi.json\n- scope: onboarding.merchant.write\n  description: Grants read & write access to merchant onboarding related APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: onboarding.order.read\n  description: Grants read access to onboarding orders related APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: onboarding.order.write\n  description: Grants read & write access to onboarding orders related APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: payment.read\n  description: Grants read access to payment related APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: payment.write\n  description: Grants read & write access to payment related APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n\
  - scope: refund.read\n  description: Grants read access to refunds\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n- scope: refund.write\n  description: Grants read & write access to refunds\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moneris-unified-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/scopes/moneris-scopes.yml
summary_line: 14 scopes · clientCredentials
tags:
- Financial-Services
- Payments
- Payment Processing
- Card Payments
- Merchant Services
- Acquiring
- Canada
- Fintech
- Infrastructure
token_urls:
- /oauth2/token
---
