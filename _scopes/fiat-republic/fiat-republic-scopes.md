---
authorization_urls: []
description: ''
docs: https://docs.fiatrepublic.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fiat Republic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fiat Republic publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fiat Republic API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fiat Republic
provider_slug: fiat-republic
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - https://docs.fiatrepublic.com/docs/authentication
  tokenUrl: https://sandbox.fiatrepublic.com/passport/oauth/token
scope_count: 2
scope_names:
- PAYMENTS
- OXYGEN
scopes:
- description: Access to the core payments product surface (end users, fiat and virtual accounts, payees, payments, returns, conversions, webhooks, documents). Requested at token time; expands to "PAYMENTS payments.*".
  flows:
  - clientCredentials
  scope: PAYMENTS
- description: Access to the Oxygen transaction-monitoring product (entities, payment channels, transactions, rules, investigations, Oxygen webhooks). Requested with a separate access token.
  flows:
  - clientCredentials
  scope: OXYGEN
slug: fiat-republic-scopes
source_filename: fiat-republic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fiatrepublic.com/docs/authentication\ndocs: https://docs.fiatrepublic.com/docs/authentication\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  tokenUrl: https://sandbox.fiatrepublic.com/passport/oauth/token\n  sources: [https://docs.fiatrepublic.com/docs/authentication]\nscopes:\n- scope: PAYMENTS\n  description: >-\n    Access to the core payments product surface (end users, fiat and virtual accounts, payees,\n    payments, returns, conversions, webhooks, documents). Requested at token time; expands to\n    \"PAYMENTS payments.*\".\n  flows: [clientCredentials]\n  sources: [https://docs.fiatrepublic.com/docs/authentication]\n- scope: OXYGEN\n  description: >-\n    Access to the Oxygen transaction-monitoring product (entities, payment channels,\n    transactions, rules, investigations, Oxygen webhooks). Requested with a separate access token.\n  flows: [clientCredentials]\n  sources: [https://docs.fiatrepublic.com/docs/authentication]\n\
  notes: >-\n  Fiat Republic issues coarse-grained product scopes (PAYMENTS, OXYGEN) rather than per-resource\n  read/write scopes; a token is minted per product surface via the client-credentials flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiat-republic/refs/heads/main/scopes/fiat-republic-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Banking
- Payments
- Fintech
- Cryptocurrency
- Stablecoins
- Banking-as-a-Service
- Embedded Finance
- Compliance
- KYC
- SEPA
- Faster Payments
token_urls: []
---
