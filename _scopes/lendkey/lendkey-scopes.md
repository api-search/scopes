---
api_specs:
- filename: lendkey-integration-openapi.yml
  format: yaml
  label: LendKey Integration API
  slug: integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-integration-openapi.yml
- filename: lendkey-treasury-management-openapi.yml
  format: yaml
  label: LendKey Treasury Management API
  slug: treasury-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-treasury-management-openapi.yml
- filename: lendkey-esign-openapi.yml
  format: yaml
  label: LendKey E-Sign API
  slug: esign
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-esign-openapi.yml
- filename: lendkey-partner-integration-internal-openapi.yml
  format: yaml
  label: LendKey Partner Integration Internal API
  slug: partner-integration-internal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-partner-integration-internal-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lendkey Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LendKey uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LendKey
provider_slug: lendkey
schemes:
- description: OAuth2 client credentials flow via Kong Gateway
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/lendkey-esign-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token
  name: oauth2
  source: openapi/lendkey-partner-integration-internal-openapi.yml
- description: OAuth2 client credentials flow via Kong Gateway
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/lendkey-treasury-management-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: lendkey-scopes
source_filename: lendkey-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lendkey-esign-openapi.yml, openapi/lendkey-partner-integration-internal-openapi.yml,\n  openapi/lendkey-treasury-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/lendkey-esign-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: OAuth2 client credentials flow via Kong Gateway\n- name: oauth2\n  source: openapi/lendkey-partner-integration-internal-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token\n- name: oauth2\n  source: openapi/lendkey-treasury-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: OAuth2 client credentials flow via Kong Gateway\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/scopes/lendkey-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Lending
- Loans
- Student Loans
- Credit Unions
- Banking
- Loan Origination
- Financial Services
- Payments
- E-Signature
- Treasury
token_urls:
- /oauth2/token
- https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token
---
