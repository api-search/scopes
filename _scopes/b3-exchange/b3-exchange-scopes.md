---
api_specs:
- filename: b3-exchange-investor-position-openapi.json
  format: json
  label: B3 Investor Area (Área do Investidor) APIs
  slug: b3-investor-area-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-investor-position-openapi.json
- filename: b3-exchange-tesouro-direto-bonds-openapi.json
  format: json
  label: B3 Tesouro Direto APIs
  slug: b3-tesouro-direto-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-tesouro-direto-bonds-openapi.json
- filename: b3-exchange-otc-public-info-openapi.json
  format: json
  label: B3 OTC (Balcão) APIs
  slug: b3-otc-balcao-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-otc-public-info-openapi.json
- filename: b3-exchange-core-calculation-openapi.json
  format: json
  label: B3 Listed Markets (Listados) APIs
  slug: b3-listed-markets-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-core-calculation-openapi.json
- filename: b3-exchange-isin-openapi.json
  format: json
  label: B3 ISIN API
  slug: b3-isin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-isin-openapi.json
- filename: b3-exchange-banco-b3-custody-openapi.json
  format: json
  label: Banco B3 APIs
  slug: b3-banco-b3-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-banco-b3-custody-openapi.json
- filename: b3-exchange-insurance-claim-openapi.json
  format: json
  label: B3 Insurance (Seguros) APIs
  slug: b3-insurance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-insurance-claim-openapi.json
- filename: b3-exchange-auth-client-credentials-openapi.json
  format: json
  label: B3 Authentication APIs
  slug: b3-authentication-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-auth-client-credentials-openapi.json
authorization_urls: []
description: ''
docs: https://developers.b3.com.br/apis/autenticacao
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: derived
name: B3 Exchange Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'B3 (Brasil Bolsa Balcão) publishes 2 OAuth 2.0 scopes via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the B3 (Brasil Bolsa Balcão) API on a user''s behalf.


  Tokens are issued from https://localhost:8089/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: B3 (Brasil Bolsa Balcão)
provider_slug: b3-exchange
schemes:
- flows:
  - flow: clientCredentials
    note: Placeholder host in the published Swagger definitions - the portal substitutes the client's entitled gateway host at runtime. The documented token model APIs POST to /aapi/oauth/token (client credentials) and /api/oauth/token (ROPC).
    tokenUrl: https://localhost:8089/api/oauth/token
  - flow: password
    note: Resource Owner Password Credentials model APIs (plain and category_ID variants).
  name: OAuth2
  type: oauth2
scope_count: 2
scope_names:
- resource.READ
- resource.WRITE
scopes:
- description: Read access to the API resource (portal-wide OAuth 2.0 security profile, any-scope matching).
  flows:
  - clientCredentials
  - password
  scope: resource.READ
- description: Write access to the API resource (portal-wide OAuth 2.0 security profile, any-scope matching).
  flows:
  - clientCredentials
  - password
  scope: resource.WRITE
slug: b3-exchange-scopes
source_filename: b3-exchange-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: derived\nsource: openapi/ (Swagger 1.1 authorizations + securityProfile blocks, 12 of 14 definitions)\ndocs: https://developers.b3.com.br/apis/autenticacao\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://localhost:8089/api/oauth/token\n        note: >-\n          Placeholder host in the published Swagger definitions - the portal\n          substitutes the client's entitled gateway host at runtime. The\n          documented token model APIs POST to /aapi/oauth/token (client\n          credentials) and /api/oauth/token (ROPC).\n      - flow: password\n        note: Resource Owner Password Credentials model APIs (plain and category_ID variants).\nscopes:\n  - scope: resource.READ\n    description: Read access to the API resource (portal-wide OAuth 2.0 security profile, any-scope matching).\n    flows: [clientCredentials, password]\n    sources:\n      - openapi/ (12 harvested\
  \ Swagger 1.1 definitions)\n  - scope: resource.WRITE\n    description: Write access to the API resource (portal-wide OAuth 2.0 security profile, any-scope matching).\n    flows: [clientCredentials, password]\n    sources:\n      - openapi/ (12 harvested Swagger 1.1 definitions)\nnotes: >-\n  B3 uses a coarse two-scope model (resource.READ / resource.WRITE) applied\n  uniformly across the developer-portal catalog rather than per-product scopes.\n  Some Client Credentials variants add a category_ID, key, or scope request\n  parameter at the token endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/scopes/b3-exchange-scopes.yml
summary_line: 2 scopes · clientCredentials/password
tags:
- Financial
- Market Data
- Stocks
- Trading
- Exchange
- Derivatives
- Fixed Income
- Real-Time
- Reference Data
- Brazil
token_urls:
- https://localhost:8089/api/oauth/token
---
