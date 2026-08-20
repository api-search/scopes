---
api_specs:
- filename: upward-financial-accounts-api-openapi.yml
  format: yaml
  label: Upward Financial accounts API
  slug: upward-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-accounts-api-openapi.yml
- filename: upward-financial-auth-api-openapi.yml
  format: yaml
  label: Upward Financial auth API
  slug: upward-financial-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-auth-api-openapi.yml
- filename: upward-financial-billpayments-api-openapi.yml
  format: yaml
  label: Upward Financial billPayments API
  slug: upward-financial-billpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billpayments-api-openapi.yml
- filename: upward-financial-billreporting-api-openapi.yml
  format: yaml
  label: Upward Financial billReporting API
  slug: upward-financial-billreporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billreporting-api-openapi.yml
- filename: upward-financial-billswitch-api-openapi.yml
  format: yaml
  label: Upward Financial billSwitch API
  slug: upward-financial-billswitch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-billswitch-api-openapi.yml
- filename: upward-financial-cbaas-api-openapi.yml
  format: yaml
  label: Upward Financial cbaas API
  slug: upward-financial-cbaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-cbaas-api-openapi.yml
- filename: upward-financial-consumers-api-openapi.yml
  format: yaml
  label: Upward Financial consumers API
  slug: upward-financial-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-consumers-api-openapi.yml
- filename: upward-financial-creditinsights-api-openapi.yml
  format: yaml
  label: Upward Financial creditInsights API
  slug: upward-financial-creditinsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-creditinsights-api-openapi.yml
- filename: upward-financial-onboarding-api-openapi.yml
  format: yaml
  label: Upward Financial onboarding API
  slug: upward-financial-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-onboarding-api-openapi.yml
- filename: upward-financial-partners-api-openapi.yml
  format: yaml
  label: Upward Financial partners API
  slug: upward-financial-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-partners-api-openapi.yml
- filename: upward-financial-paymentcards-api-openapi.yml
  format: yaml
  label: Upward Financial paymentCards API
  slug: upward-financial-paymentcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-paymentcards-api-openapi.yml
- filename: upward-financial-payments-api-openapi.yml
  format: yaml
  label: Upward Financial payments API
  slug: upward-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-payments-api-openapi.yml
- filename: upward-financial-plaid-api-openapi.yml
  format: yaml
  label: Upward Financial plaid API
  slug: upward-financial-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-plaid-api-openapi.yml
- filename: upward-financial-rewards-api-openapi.yml
  format: yaml
  label: Upward Financial rewards API
  slug: upward-financial-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-rewards-api-openapi.yml
- filename: upward-financial-simulations-api-openapi.yml
  format: yaml
  label: Upward Financial simulations API
  slug: upward-financial-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-simulations-api-openapi.yml
- filename: upward-financial-statements-api-openapi.yml
  format: yaml
  label: Upward Financial statements API
  slug: upward-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-statements-api-openapi.yml
- filename: upward-financial-webhooks-api-openapi.yml
  format: yaml
  label: Upward Financial webhooks API
  slug: upward-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/openapi/upward-financial-webhooks-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scopes for the Upward (Upwardli) Credit Suite API, captured from the developer portal's authentication and token-exchange documentation. The OpenAPI itself only declares the resulting Bearer scheme, so this scope reference is sourced from the docs. Partner (M2M) tokens are requested via client_credentials; consumer-scoped tokens are minted via RFC 8693 token exchange using the dynamic consumer:<upward_consumer_id> scope.
docs: https://developers.upwardli.com/concepts/authentication/o-auth-2-0
flows:
- clientCredentials
- token-exchange (urn:ietf:params:oauth:grant-type:token-exchange)
kind: oauth-scopes
layout: scope
method: searched
name: Upward Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upward Financial publishes 9 OAuth 2.0 scopes via the clientCredentials and token-exchange (urn:ietf:params:oauth:grant-type:token-exchange) flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upward Financial API on a user''s behalf.


  Tokens are issued from https://auth.upwardli.com/auth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upward Financial
provider_slug: upward-financial
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.upwardli.com/auth/token/
  name: oauth2ClientCredentials
  source: https://developers.upwardli.com/concepts/authentication/o-auth-2-0
- flows:
  - flow: token-exchange (urn:ietf:params:oauth:grant-type:token-exchange)
    tokenUrl: https://auth.upwardli.com/auth/token/exchange/
  name: oauth2TokenExchange
  source: https://developers.upwardli.com/concepts/authentication/token-exchange
scope_count: 9
scope_names:
- api:read
- api:write
- ui:client-onboarding
- api:credit-insights:read
- api:profile:read
- api:trade-line:read
- api:rewards:read
- api:rewards:write
- consumer:<upward_consumer_id>
scopes:
- description: Perform read-only operations for machine to machine (M2M) scenarios.
  flows:
  - clientCredentials
  - token-exchange
  scope: api:read
- description: Perform full CRUD operations for machine to machine (M2M) scenarios.
  flows:
  - clientCredentials
  - token-exchange
  scope: api:write
- description: Used for the Onboarding Client Component in combination with api:read and api:write.
  flows:
  - clientCredentials
  - token-exchange
  scope: ui:client-onboarding
- description: Access to read Credit Insights data.
  flows:
  - clientCredentials
  - token-exchange
  scope: api:credit-insights:read
- description: Access to read Profile data.
  flows:
  - clientCredentials
  - token-exchange
  scope: api:profile:read
- description: Access to read Credit Line (trade line) data.
  flows:
  - clientCredentials
  - token-exchange
  scope: api:trade-line:read
- description: Access to read Cashback Rewards configurations, enrollments, and offers.
  flows:
  - clientCredentials
  scope: api:rewards:read
- description: Access to enroll a card in Cashback Rewards.
  flows:
  - clientCredentials
  scope: api:rewards:write
- description: Dynamic scope granted via token exchange only — read and write data for a specific consumer. The resulting limited token is safe to send to the client application/web browser.
  flows:
  - token-exchange
  scope: consumer:<upward_consumer_id>
slug: upward-financial-scopes
source_filename: upward-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.upwardli.com/concepts/authentication/o-auth-2-0\ndocs: https://developers.upwardli.com/concepts/authentication/o-auth-2-0\ndescription: >-\n  OAuth 2.0 scopes for the Upward (Upwardli) Credit Suite API, captured from\n  the developer portal's authentication and token-exchange documentation. The\n  OpenAPI itself only declares the resulting Bearer scheme, so this scope\n  reference is sourced from the docs. Partner (M2M) tokens are requested via\n  client_credentials; consumer-scoped tokens are minted via RFC 8693 token\n  exchange using the dynamic consumer:<upward_consumer_id> scope.\nschemes:\n- name: oauth2ClientCredentials\n  source: https://developers.upwardli.com/concepts/authentication/o-auth-2-0\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.upwardli.com/auth/token/\n- name: oauth2TokenExchange\n  source: https://developers.upwardli.com/concepts/authentication/token-exchange\n\
  \  flows:\n  - flow: token-exchange (urn:ietf:params:oauth:grant-type:token-exchange)\n    tokenUrl: https://auth.upwardli.com/auth/token/exchange/\nscopes:\n- scope: api:read\n  description: Perform read-only operations for machine to machine (M2M) scenarios.\n  flows: [clientCredentials, token-exchange]\n- scope: api:write\n  description: Perform full CRUD operations for machine to machine (M2M) scenarios.\n  flows: [clientCredentials, token-exchange]\n- scope: ui:client-onboarding\n  description: >-\n    Used for the Onboarding Client Component in combination with api:read and\n    api:write.\n  flows: [clientCredentials, token-exchange]\n- scope: api:credit-insights:read\n  description: Access to read Credit Insights data.\n  flows: [clientCredentials, token-exchange]\n- scope: api:profile:read\n  description: Access to read Profile data.\n  flows: [clientCredentials, token-exchange]\n- scope: api:trade-line:read\n  description: Access to read Credit Line (trade line) data.\n  flows:\
  \ [clientCredentials, token-exchange]\n- scope: api:rewards:read\n  description: >-\n    Access to read Cashback Rewards configurations, enrollments, and offers.\n  flows: [clientCredentials]\n- scope: api:rewards:write\n  description: Access to enroll a card in Cashback Rewards.\n  flows: [clientCredentials]\n- scope: consumer:<upward_consumer_id>\n  description: >-\n    Dynamic scope granted via token exchange only — read and write data for a\n    specific consumer. The resulting limited token is safe to send to the\n    client application/web browser.\n  flows: [token-exchange]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upward-financial/refs/heads/main/scopes/upward-financial-scopes.yml
summary_line: 9 scopes · clientCredentials/token-exchange (urn:ietf:params:oauth:grant-type:token-exchange)
tags:
- Company
- Fintech
- Credit
- Credit Building
- Payments
- Cards
- Embedded Finance
- Bill Pay
- Banking
- KYC
token_urls:
- https://auth.upwardli.com/auth/token/
- https://auth.upwardli.com/auth/token/exchange/
---
