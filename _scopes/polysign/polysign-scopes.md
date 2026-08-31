---
api_specs:
- filename: polysign-abc-accounts-api-openapi.yml
  format: yaml
  label: PolySign ABC Accounts API
  slug: polysign-abc-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-accounts-api-openapi.yml
- filename: polysign-abc-memorials-api-openapi.yml
  format: yaml
  label: PolySign ABC Memorials API
  slug: polysign-abc-memorials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-memorials-api-openapi.yml
- filename: polysign-abc-signing-api-openapi.yml
  format: yaml
  label: PolySign ABC Signing API
  slug: polysign-abc-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-signing-api-openapi.yml
- filename: polysign-abc-testnet-api-openapi.yml
  format: yaml
  label: PolySign ABC Testnet API
  slug: polysign-abc-testnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-abc-testnet-api-openapi.yml
- filename: polysign-asset-api-openapi.yml
  format: yaml
  label: PolySign Asset API
  slug: polysign-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-asset-api-openapi.yml
- filename: polysign-authentication-api-openapi.yml
  format: yaml
  label: PolySign Authentication API
  slug: polysign-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-authentication-api-openapi.yml
- filename: polysign-beneficiary-authorization-api-openapi.yml
  format: yaml
  label: PolySign beneficiary authorization API
  slug: polysign-beneficiary-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-beneficiary-authorization-api-openapi.yml
- filename: polysign-book-transfer-api-openapi.yml
  format: yaml
  label: PolySign book transfer API
  slug: polysign-book-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-api-openapi.yml
- filename: polysign-book-transfer-confirmation-api-openapi.yml
  format: yaml
  label: PolySign book transfer confirmation API
  slug: polysign-book-transfer-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-book-transfer-confirmation-api-openapi.yml
- filename: polysign-escrow-authorization-api-openapi.yml
  format: yaml
  label: PolySign escrow authorization API
  slug: polysign-escrow-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-escrow-authorization-api-openapi.yml
- filename: polysign-investor-api-openapi.yml
  format: yaml
  label: PolySign Investor API
  slug: polysign-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-investor-api-openapi.yml
- filename: polysign-order-api-openapi.yml
  format: yaml
  label: PolySign Order API
  slug: polysign-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-order-api-openapi.yml
- filename: polysign-partner-api-openapi.yml
  format: yaml
  label: PolySign Partner API
  slug: polysign-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-partner-api-openapi.yml
- filename: polysign-settlement-api-openapi.yml
  format: yaml
  label: PolySign Settlement API
  slug: polysign-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-api-openapi.yml
- filename: polysign-settlement-confirmation-api-openapi.yml
  format: yaml
  label: PolySign settlement confirmation API
  slug: polysign-settlement-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-settlement-confirmation-api-openapi.yml
- filename: polysign-system-api-openapi.yml
  format: yaml
  label: PolySign System API
  slug: polysign-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-system-api-openapi.yml
- filename: polysign-utility-api-openapi.yml
  format: yaml
  label: PolySign Utility API
  slug: polysign-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/openapi/polysign-utility-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Polysign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PolySign publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PolySign API on a user''s behalf.


  Tokens are issued from /v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PolySign
provider_slug: polysign
schemes:
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-abc-proxy-service-openapi.json
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-atomicnet-api-server-openapi.json
- description: OAuth 2.0 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: OAuth2
  source: openapi/polysign-merchant-gate-openapi.json
scope_count: 1
scope_names:
- participant
scopes:
- description: Grants access to participant.
  flows:
  - clientCredentials
  scope: participant
slug: polysign-scopes
source_filename: polysign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/polysign-abc-proxy-service-openapi.json, openapi/polysign-atomicnet-api-server-openapi.json,\n  openapi/polysign-merchant-gate-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/polysign-abc-proxy-service-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\n- name: OAuth2\n  source: openapi/polysign-atomicnet-api-server-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\n- name: OAuth2\n  source: openapi/polysign-merchant-gate-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n  description: OAuth 2.0 with the client credentials grant flow.\nscopes:\n- scope: participant\n  description: Grants access to participant.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/polysign-abc-proxy-service-openapi.json\n\
  \  - openapi/polysign-atomicnet-api-server-openapi.json\n  - openapi/polysign-merchant-gate-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polysign/refs/heads/main/scopes/polysign-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- digital-assets
- Blockchain
- Institutional Custody
- settlement
- escrow
- capital-markets
- Payments
- Fintech
- distributed-ledger
- atomicnet
token_urls:
- /v1/auth/token
---
