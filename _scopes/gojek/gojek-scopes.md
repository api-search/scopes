---
authorization_urls:
- https://integration-goauth.gojekapi.com/oauth2/auth
description: ''
docs: https://developer.gobiz.com/docs/api/auth/direct-integration/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Gojek Scopes
name_suffix: OAuth Scopes
note: Derived from the published GoBiz scope reference tables, not from an OpenAPI document - Gojek publishes no machine-readable spec. The client-credentials table on the Direct Integration page lists 18 scopes; the Facilitator (authorization code) table adds the two OpenID Connect scopes below.
overview: 'GoJek publishes 20 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the GoJek API on a user''s behalf.


  Tokens are issued from https://accounts.go-jek.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoJek
provider_slug: gojek
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.go-jek.com/oauth2/token
    tokenUrlSandbox: https://integration-goauth.gojekapi.com/oauth2/token
  name: go_auth_client_credentials
- flows:
  - authorizationUrl: https://integration-goauth.gojekapi.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.go-jek.com/oauth2/token
  name: go_auth_authorization_code
scope_count: 20
scope_names:
- openid
- offline
- partner:outlet:read
- partner:outlet:write
- gofood:catalog:read
- gofood:catalog:write
- gofood:order:read
- gofood:order:write
- gofood:outlet:write
- promo:food_promo:read
- promo:food_promo:write
- payment:transaction:read
- payment:transaction:write
- payment:pop:read
- mokapos:library:read
- mokapos:transaction:read
- mokapos:reporting:read
- mokapos:customer:read
- mokapos:checkout:write
- mokapos:salestype:read
scopes:
- description: To read basic token info.
  flows:
  - authorizationCode
  scope: openid
- description: To regenerate access token (refresh token).
  flows:
  - authorizationCode
  scope: offline
- description: To read outlet data.
  flows:
  - clientCredentials
  - authorizationCode
  scope: partner:outlet:read
- description: To edit or update outlet data.
  flows:
  - clientCredentials
  - authorizationCode
  scope: partner:outlet:write
- description: To read GoFood menu.
  flows:
  - clientCredentials
  - authorizationCode
  scope: gofood:catalog:read
- description: To modify GoFood menu.
  flows:
  - clientCredentials
  - authorizationCode
  scope: gofood:catalog:write
- description: To read GoFood order data.
  flows:
  - clientCredentials
  - authorizationCode
  scope: gofood:order:read
- description: To mark an order is ready.
  flows:
  - clientCredentials
  - authorizationCode
  scope: gofood:order:write
- description: To modify restaurant properties.
  flows:
  - clientCredentials
  scope: gofood:outlet:write
- description: To retrieve GoFood promotions.
  flows:
  - clientCredentials
  scope: promo:food_promo:read
- description: To modify GoFood promotions.
  flows:
  - clientCredentials
  scope: promo:food_promo:write
- description: To read payment transaction.
  flows:
  - clientCredentials
  scope: payment:transaction:read
- description: To modify payment transaction.
  flows:
  - clientCredentials
  scope: payment:transaction:write
- description: To read payment PoP (proof of payment) data.
  flows:
  - clientCredentials
  scope: payment:pop:read
- description: To read MokaPOS library data.
  flows:
  - clientCredentials
  scope: mokapos:library:read
- description: To read MokaPOS transaction data.
  flows:
  - clientCredentials
  scope: mokapos:transaction:read
- description: To read MokaPOS reporting data.
  flows:
  - clientCredentials
  scope: mokapos:reporting:read
- description: To read MokaPOS customer data.
  flows:
  - clientCredentials
  scope: mokapos:customer:read
- description: To update MokaPOS checkout data.
  flows:
  - clientCredentials
  scope: mokapos:checkout:write
- description: To read MokaPOS sales type data.
  flows:
  - clientCredentials
  scope: mokapos:salestype:read
slug: gojek-scopes
source_filename: gojek-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://developer.gobiz.com/docs/api/auth/direct-integration/\ndocs: https://developer.gobiz.com/docs/api/auth/direct-integration/\nnote: >-\n  Derived from the published GoBiz scope reference tables, not from an OpenAPI\n  document - Gojek publishes no machine-readable spec. The client-credentials\n  table on the Direct Integration page lists 18 scopes; the Facilitator\n  (authorization code) table adds the two OpenID Connect scopes below.\nschemes:\n- name: go_auth_client_credentials\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.go-jek.com/oauth2/token\n    tokenUrlSandbox: https://integration-goauth.gojekapi.com/oauth2/token\n- name: go_auth_authorization_code\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://integration-goauth.gojekapi.com/oauth2/auth\n    tokenUrl: https://accounts.go-jek.com/oauth2/token\nscopes:\n- {scope: 'openid', description: 'To read basic token info.',\
  \ flows: [authorizationCode]}\n- {scope: 'offline', description: 'To regenerate access token (refresh token).', flows: [authorizationCode]}\n- {scope: 'partner:outlet:read', description: 'To read outlet data.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'partner:outlet:write', description: 'To edit or update outlet data.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'gofood:catalog:read', description: 'To read GoFood menu.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'gofood:catalog:write', description: 'To modify GoFood menu.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'gofood:order:read', description: 'To read GoFood order data.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'gofood:order:write', description: 'To mark an order is ready.', flows: [clientCredentials, authorizationCode]}\n- {scope: 'gofood:outlet:write', description: 'To modify restaurant properties.', flows: [clientCredentials]}\n- {scope: 'promo:food_promo:read',\
  \ description: 'To retrieve GoFood promotions.', flows: [clientCredentials]}\n- {scope: 'promo:food_promo:write', description: 'To modify GoFood promotions.', flows: [clientCredentials]}\n- {scope: 'payment:transaction:read', description: 'To read payment transaction.', flows: [clientCredentials]}\n- {scope: 'payment:transaction:write', description: 'To modify payment transaction.', flows: [clientCredentials]}\n- {scope: 'payment:pop:read', description: 'To read payment PoP (proof of payment) data.', flows: [clientCredentials]}\n- {scope: 'mokapos:library:read', description: 'To read MokaPOS library data.', flows: [clientCredentials]}\n- {scope: 'mokapos:transaction:read', description: 'To read MokaPOS transaction data.', flows: [clientCredentials]}\n- {scope: 'mokapos:reporting:read', description: 'To read MokaPOS reporting data.', flows: [clientCredentials]}\n- {scope: 'mokapos:customer:read', description: 'To read MokaPOS customer data.', flows: [clientCredentials]}\n- {scope: 'mokapos:checkout:write',\
  \ description: 'To update MokaPOS checkout data.', flows: [clientCredentials]}\n- {scope: 'mokapos:salestype:read', description: 'To read MokaPOS sales type data.', flows: [clientCredentials]}\nscope_count: 20\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojek/refs/heads/main/scopes/gojek-scopes.yml
summary_line: 20 scopes · clientCredentials/authorizationCode
tags:
- Company
- Super App
- Ride Hailing
- Food Delivery
- Point of Sale
- Merchant Platform
- Payments
- QRIS
- Logistics
- Indonesia
- Southeast Asia
- Webhooks
- OAuth
token_urls:
- https://accounts.go-jek.com/oauth2/token
---
