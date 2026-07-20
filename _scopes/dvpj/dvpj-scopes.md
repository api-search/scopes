---
authorization_urls:
- https://auth.contaazul.com/login
description: ''
docs: https://developers.contaazul.com/requestingcode
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Dvpj Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Conta Azul publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conta Azul API on a user''s behalf.


  Tokens are issued from https://auth.contaazul.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conta Azul
provider_slug: dvpj
schemes:
- flows:
  - authorizationUrl: https://auth.contaazul.com/login
    flow: authorizationCode
    tokenUrl: https://auth.contaazul.com/oauth2/token
  name: OAuth2
scope_count: 3
scope_names:
- openid
- profile
- aws.cognito.signin.user.admin
scopes:
- description: OpenID Connect base scope; issues an ID token identifying the authenticated Conta Azul user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: AWS Cognito user-admin scope. In Conta Azul this grants the application administrator-level access to the connected ERP account's resources (per the docs, "seu aplicativo terá a permissão de administrador").
  flows:
  - authorizationCode
  scope: aws.cognito.signin.user.admin
slug: dvpj-scopes
source_filename: dvpj-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.contaazul.com/requestingcode\ndocs: https://developers.contaazul.com/requestingcode\nprovider_oauth: AWS Cognito hosted UI\nschemes:\n  - name: OAuth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.contaazul.com/login\n        tokenUrl: https://auth.contaazul.com/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect base scope; issues an ID token identifying the authenticated Conta Azul user.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the authenticated user's basic profile claims.\n    flows: [authorizationCode]\n  - scope: aws.cognito.signin.user.admin\n    description: >-\n      AWS Cognito user-admin scope. In Conta Azul this grants the application\n      administrator-level access to the connected ERP account's resources\n      (per the docs, \"seu aplicativo terá a permissão de administrador\").\n    flows:\
  \ [authorizationCode]\nnotes: >-\n  Conta Azul does not publish a granular per-resource scope catalog; the single\n  requested scope string is `openid profile aws.cognito.signin.user.admin`,\n  which grants the integration admin access to the connected account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dvpj/refs/heads/main/scopes/dvpj-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- ERP
- Financial
- Accounting
- Invoicing
- Payments
- SMB
- Brazil
- OAuth
token_urls:
- https://auth.contaazul.com/oauth2/token
---
