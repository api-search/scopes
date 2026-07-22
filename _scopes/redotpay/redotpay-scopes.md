---
authorization_urls: []
description: OAuth2 scopes used by RedotPay agentic payments. Derived from the first-party redotpay CLI / redotpay-payment configuration and skill (no public OpenAPI or scopes reference page is published).
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Redotpay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Redotpay uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Redotpay
provider_slug: redotpay
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: redotpay-scopes
source_filename: redotpay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/redotpay/redotpay-cli (config.example.toml, SKILL.md CLI appendix)\ndescription: >-\n  OAuth2 scopes used by RedotPay agentic payments. Derived from the first-party redotpay CLI /\n  redotpay-payment configuration and skill (no public OpenAPI or scopes reference page is published).\noauth_flow: device_authorization\nscopes:\n- name: mpp_charge\n  description: >-\n    Authorize the client/agent to settle Machine Payments Protocol (MPP) charges on the user's behalf\n    (e.g. `redotpay-payment auth start --scope mpp_charge`). Grants the ability to obtain a payment\n    credential and complete 402 payments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redotpay/refs/heads/main/scopes/redotpay-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Payments
- Fintech
- Stablecoin
- Cryptocurrency
- Wallet
- Agentic Payments
- Machine Payments Protocol
- x402
- OAuth
token_urls: []
---
