---
api_specs:
- filename: tango-card-accounts-api-openapi.yml
  format: yaml
  label: Tango Card Accounts API
  slug: tango-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-accounts-api-openapi.yml
- filename: tango-card-brand-categories-api-openapi.yml
  format: yaml
  label: Tango Card Brand Categories API
  slug: tango-card-brand-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-brand-categories-api-openapi.yml
- filename: tango-card-catalog-api-openapi.yml
  format: yaml
  label: Tango Card Catalog API
  slug: tango-card-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-catalog-api-openapi.yml
- filename: tango-card-choice-products-api-openapi.yml
  format: yaml
  label: Tango Card Choice Products API
  slug: tango-card-choice-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-choice-products-api-openapi.yml
- filename: tango-card-countries-currencies-api-openapi.yml
  format: yaml
  label: Tango Card Countries & Currencies API
  slug: tango-card-countries-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-countries-currencies-api-openapi.yml
- filename: tango-card-credential-types-api-openapi.yml
  format: yaml
  label: Tango Card Credential Types API
  slug: tango-card-credential-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-credential-types-api-openapi.yml
- filename: tango-card-customers-api-openapi.yml
  format: yaml
  label: Tango Card Customers API
  slug: tango-card-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-customers-api-openapi.yml
- filename: tango-card-digital-templates-api-openapi.yml
  format: yaml
  label: Tango Card Digital Templates API
  slug: tango-card-digital-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-digital-templates-api-openapi.yml
- filename: tango-card-exchange-rates-api-openapi.yml
  format: yaml
  label: Tango Card Exchange Rates API
  slug: tango-card-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-exchange-rates-api-openapi.yml
- filename: tango-card-fund-management-api-openapi.yml
  format: yaml
  label: Tango Card Fund Management API
  slug: tango-card-fund-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-fund-management-api-openapi.yml
- filename: tango-card-line-items-api-openapi.yml
  format: yaml
  label: Tango Card Line Items API
  slug: tango-card-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-line-items-api-openapi.yml
- filename: tango-card-low-balance-alerts-api-openapi.yml
  format: yaml
  label: Tango Card Low Balance Alerts API
  slug: tango-card-low-balance-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-low-balance-alerts-api-openapi.yml
- filename: tango-card-orders-api-openapi.yml
  format: yaml
  label: Tango Card Orders API
  slug: tango-card-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/openapi/tango-card-orders-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.tangocard.com/docs/acquire-service-account-token
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Tango Card Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tango Card publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tango Card API on a user''s behalf.


  Tokens are issued from https://auth.tangocard.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tango Card
provider_slug: tango-card
schemes:
- description: OAuth 2.0 client credentials flow for more secure integrations
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tangocard.com/oauth/token
  name: oAuth2
  source: openapi/tango-raas-api-openapi.yml
scope_count: 1
scope_names:
- raas.all
scopes:
- description: The single static scope for the Tango RaaS API; the docs state the scope value is always raas.all, granting access to all Rewards as a Service permissions. No granular scopes are published.
  flows: []
  scope: raas.all
slug: tango-card-scopes
source_filename: tango-card-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/tango-raas-api-openapi.yml\ndocs: https://developers.tangocard.com/docs/acquire-service-account-token\nschemes:\n- name: oAuth2\n  source: openapi/tango-raas-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tangocard.com/oauth/token\n  description: OAuth 2.0 client credentials flow for more secure integrations\nscopes:\n- scope: raas.all\n  description: The single static scope for the Tango RaaS API; the docs state the\n    scope value is always raas.all, granting access to all Rewards as a Service\n    permissions. No granular scopes are published.\n  sources:\n  - https://developers.tangocard.com/docs/acquire-service-account-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/scopes/tango-card-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Gift Cards
- Rewards
- Incentives
- Digital Rewards
- Prepaid Cards
- Payments
token_urls:
- https://auth.tangocard.com/oauth/token
---
