---
authorization_urls:
- https://auth.montran.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Montran Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Montran publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Montran API on a user''s behalf.


  Tokens are issued from https://auth.montran.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Montran
provider_slug: montran
schemes:
- description: OAuth 2.0 authorization for PSD2 AISP/PISP access
  flows:
  - authorizationUrl: https://auth.montran.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.montran.com/oauth2/token
  name: oauth2
  source: openapi/montran-instant-payments-gateway-openapi.yml
scope_count: 2
scope_names:
- aisp
- pisp
scopes:
- description: Account Information Service Provider access
  flows:
  - authorizationCode
  scope: aisp
- description: Payment Initiation Service Provider access
  flows:
  - authorizationCode
  scope: pisp
slug: montran-scopes
source_filename: montran-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/montran-instant-payments-gateway-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/montran-instant-payments-gateway-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.montran.com/oauth2/authorize\n    tokenUrl: https://auth.montran.com/oauth2/token\n  description: OAuth 2.0 authorization for PSD2 AISP/PISP access\nscopes:\n- scope: aisp\n  description: Account Information Service Provider access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/montran-instant-payments-gateway-openapi.yml\n- scope: pisp\n  description: Payment Initiation Service Provider access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/montran-instant-payments-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/scopes/montran-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
token_urls:
- https://auth.montran.com/oauth2/token
---
