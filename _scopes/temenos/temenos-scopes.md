---
api_specs:
- filename: openapi.json
  format: json
  label: Temenos Transact API
  slug: temenos-transact-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/transact/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Infinity API
  slug: temenos-infinity-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/infinity/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Payments API
  slug: temenos-payments-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/payments/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Fund Administration API
  slug: temenos-fund-administration-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/funds/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Financial Crime Mitigation API
  slug: temenos-financial-crime-mitigation-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/fcm/openapi.json
- filename: temenos-data-hub-openapi.yml
  format: yaml
  label: Temenos Transact Data Hub API
  slug: temenos-transact-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-data-hub-openapi.yml
- filename: temenos-wealth-openapi.yml
  format: yaml
  label: Temenos Wealth API
  slug: temenos-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-wealth-openapi.yml
- filename: temenos-enterprise-product-pricing-openapi.yml
  format: yaml
  label: Temenos Enterprise Product and Pricing API
  slug: temenos-enterprise-product-and-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-enterprise-product-pricing-openapi.yml
- filename: temenos-cloud-banking-openapi.yml
  format: yaml
  label: Temenos Cloud Banking (CMB) API
  slug: temenos-cloud-banking-cmb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-cloud-banking-openapi.yml
- filename: temenos-journey-manager-openapi.yml
  format: yaml
  label: Temenos Journey Manager API
  slug: temenos-journey-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-journey-manager-openapi.yml
- filename: temenos-microservices-openapi.yml
  format: yaml
  label: Temenos Transact Microservices API
  slug: temenos-transact-microservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-microservices-openapi.yml
- filename: temenos-bnpl-openapi.yml
  format: yaml
  label: Temenos Buy Now Pay Later API
  slug: temenos-buy-now-pay-later-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-bnpl-openapi.yml
authorization_urls:
- https://journey.temenos.com/oauth2/authorize
- https://auth.temenos.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Temenos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Temenos publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Temenos API on a user''s behalf.


  Tokens are issued from https://journey.temenos.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Temenos
provider_slug: temenos
schemes:
- flows:
  - authorizationUrl: https://journey.temenos.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://journey.temenos.com/oauth2/token
  name: oauth2
  source: openapi/temenos-journey-manager-openapi.yml
- description: OAuth 2.0 authentication for API access
  flows:
  - authorizationUrl: https://auth.temenos.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.temenos.com/oauth2/token
  name: oauth2
  source: openapi/temenos-transact-openapi.yml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Administrative access
  flows:
  - authorizationCode
  scope: admin
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: temenos-scopes
source_filename: temenos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temenos-journey-manager-openapi.yml, openapi/temenos-transact-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/temenos-journey-manager-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://journey.temenos.com/oauth2/authorize\n    tokenUrl: https://journey.temenos.com/oauth2/token\n- name: oauth2\n  source: openapi/temenos-transact-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.temenos.com/oauth2/authorize\n    tokenUrl: https://auth.temenos.com/oauth2/token\n  description: OAuth 2.0 authentication for API access\nscopes:\n- scope: admin\n  description: Administrative access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-transact-openapi.yml\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n- scope:\
  \ write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/scopes/temenos-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
token_urls:
- https://journey.temenos.com/oauth2/token
- https://auth.temenos.com/oauth2/token
---
