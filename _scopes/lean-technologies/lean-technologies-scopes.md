---
api_specs:
- filename: lean-technologies-account-on-file-openapi.yml
  format: yaml
  label: Lean UAE Open Finance & Payments
  slug: lean-uae-open-finance-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-account-on-file-openapi.yml
- filename: lean-technologies-ksa-accounts-access-consents-openapi.yml
  format: yaml
  label: Lean KSA Open Banking
  slug: lean-ksa-open-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.leantech.me/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Lean Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lean Technologies publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lean Technologies API on a user''s behalf.


  Tokens are issued from https://auth.leantech.me/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lean Technologies
provider_slug: lean-technologies
schemes:
- flows:
  - flow: clientCredentials
    sandboxTokenUrl: https://auth.sandbox.leantech.me/oauth2/token
    tokenUrl: https://auth.leantech.me/oauth2/token
  name: OAuth2
  sources:
  - openapi/lean-technologies-payment-links-openapi.yml
  - openapi/lean-technologies-schedules-openapi.yml
  - openapi/lean-technologies-sessions-openapi.yml
scope_count: 2
scope_names:
- api
- customer.<customer_id>
scopes:
- description: Backend access to Lean's APIs (server-to-server, client_credentials).
  flows:
  - clientCredentials
  scope: api
- description: Customer-scoped access for the LinkSDK, minted per customer immediately before SDK invocation (>= 10 min validity).
  flows:
  - clientCredentials
  scope: customer.<customer_id>
slug: lean-technologies-scopes
source_filename: lean-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/lean-technologies-payment-links-openapi.yml, openapi/lean-technologies-schedules-openapi.yml, openapi/lean-technologies-sessions-openapi.yml\ndocs: https://docs.leantech.me/docs/authentication\nschemes:\n  - name: OAuth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.leantech.me/oauth2/token\n        sandboxTokenUrl: https://auth.sandbox.leantech.me/oauth2/token\n    sources:\n      - openapi/lean-technologies-payment-links-openapi.yml\n      - openapi/lean-technologies-schedules-openapi.yml\n      - openapi/lean-technologies-sessions-openapi.yml\nscopes:\n  - scope: api\n    description: Backend access to Lean's APIs (server-to-server, client_credentials).\n    flows: [clientCredentials]\n    sources: [openapi/lean-technologies-payment-links-openapi.yml]\n  - scope: customer.<customer_id>\n    description: Customer-scoped access for the LinkSDK, minted per customer immediately before SDK\
  \ invocation (>= 10 min validity).\n    flows: [clientCredentials]\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/scopes/lean-technologies-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Open Banking
- Open Finance
- Payments
- Financial Data
- Fintech
- MENA
- UAE
- Saudi Arabia
- Pay by Bank
- Bank Data
- Account Verification
- Payouts
token_urls:
- https://auth.leantech.me/oauth2/token
---
