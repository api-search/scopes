---
api_specs:
- filename: ripple-labs-rlusd-openapi-original.yml
  format: yaml
  label: Ripple Mint API (RLUSD Stablecoin)
  slug: ripple-mint-api-rlusd-stablecoin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-rlusd-openapi-original.yml
- filename: ripple-labs-ripplenet-openapi-original.yml
  format: yaml
  label: RippleNet Server API
  slug: ripplenet-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-ripplenet-openapi-original.yml
- filename: ripple-labs-report-service-openapi-original.yml
  format: yaml
  label: Report Service API
  slug: report-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-report-service-openapi-original.yml
- filename: ripple-labs-smart-liquidation-openapi-original.yml
  format: yaml
  label: Smart Liquidation API
  slug: smart-liquidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-smart-liquidation-openapi-original.yml
- filename: ripple-labs-palisade-wallet-openapi-original.yml
  format: yaml
  label: Palisade Wallet-as-a-Service API
  slug: palisade-wallet-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-palisade-wallet-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ripple Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ripple Labs publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ripple Labs API on a user''s behalf.


  Tokens are issued from https://api.ripple.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ripple Labs
provider_slug: ripple-labs
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.ripple.com/v2/oauth/token
  name: oauth2
  source: openapi/ripple-labs-rlusd-openapi-original.yml
scope_count: 2
scope_names:
- rlusd_customers:read
- rlusd_customers:write
scopes:
- description: Read transaction data
  flows:
  - clientCredentials
  scope: rlusd_customers:read
- description: Approve pending redemptions
  flows:
  - clientCredentials
  scope: rlusd_customers:write
slug: ripple-labs-scopes
source_filename: ripple-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/ripple-labs-rlusd-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/ripple-labs-rlusd-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ripple.com/v2/oauth/token\nscopes:\n- scope: rlusd_customers:read\n  description: Read transaction data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ripple-labs-rlusd-openapi-original.yml\n- scope: rlusd_customers:write\n  description: Approve pending redemptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ripple-labs-rlusd-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/scopes/ripple-labs-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Financial Services
- Payments
- Cross-Border Payments
- Blockchain
- Cryptocurrency
- Stablecoin
- Digital Assets
- Custody
- Wallet
- Fintech
token_urls:
- https://api.ripple.com/v2/oauth/token
---
