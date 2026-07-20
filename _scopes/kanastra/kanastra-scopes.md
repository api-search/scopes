---
api_specs:
- filename: kanastra-banking-openapi.yml
  format: yaml
  label: Kanastra Banking API
  slug: kanastra-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/openapi/kanastra-banking-openapi.yml
authorization_urls: []
description: ''
docs: https://banking-docs.kanastra.com.br/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Kanastra Scopes
name_suffix: OAuth Scopes
note: Kanastra issues Bearer tokens (private_key_jwt) carrying a space-delimited OAuth-style scope claim. The OpenAPI declares http bearer rather than a formal oauth2 scheme, so scopes are captured from the published token response rather than a flow scopes map.
overview: 'Kanastra publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kanastra API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kanastra
provider_slug: kanastra
schemes:
- name: bearerAuth
  source: openapi/kanastra-banking-openapi.yml
  token_endpoint: /api/v1/auth/token
scope_count: 5
scope_names:
- financial_account
- bank_slip
- bank_slip:create
- commercial_paper
- webhook
scopes:
- description: Read/manage financial (checking) accounts, balances, transactions, transfers.
  flows: []
  scope: financial_account
- description: Read/manage bank slips (boletos) and CNAB return files.
  flows: []
  scope: bank_slip
- description: Create bank slips (boletos), including batch issuance.
  flows: []
  scope: bank_slip:create
- description: Manage commercial notes (CCB), guarantees and related documents.
  flows: []
  scope: commercial_paper
- description: Subscribe to and manage webhook event delivery.
  flows: []
  scope: webhook
slug: kanastra-scopes
source_filename: kanastra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# generated: '2026-07-19'\ngenerated: '2026-07-19'\nmethod: searched\nsource: https://banking-docs.kanastra.com.br/ (token response scope claim)\ndocs: https://banking-docs.kanastra.com.br/\nnote: Kanastra issues Bearer tokens (private_key_jwt) carrying a space-delimited OAuth-style scope claim.\n  The OpenAPI declares http bearer rather than a formal oauth2 scheme, so scopes are captured from the\n  published token response rather than a flow scopes map.\nschemes:\n- name: bearerAuth\n  token_endpoint: /api/v1/auth/token\n  source: openapi/kanastra-banking-openapi.yml\nscopes:\n- scope: financial_account\n  description: Read/manage financial (checking) accounts, balances, transactions, transfers.\n- scope: bank_slip\n  description: Read/manage bank slips (boletos) and CNAB return files.\n- scope: bank_slip:create\n  description: Create bank slips (boletos), including batch issuance.\n- scope: commercial_paper\n  description: Manage commercial notes (CCB), guarantees and related\
  \ documents.\n- scope: webhook\n  description: Subscribe to and manage webhook event delivery.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/scopes/kanastra-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Banking
- Banking as a Service
- Payments
- PIX
- Boleto
- Private Credit
- Fintech
- Brazil
- Wealth Management
token_urls: []
---
