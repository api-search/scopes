---
api_specs:
- filename: conta-azul-acquittance-openapi.yml
  format: yaml
  label: Conta Azul Baixas (Acquittance)
  slug: conta-azul-baixas-acquittance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-acquittance-openapi.yml
- filename: conta-azul-charge-openapi.yml
  format: yaml
  label: Conta Azul Cobranças (Charges)
  slug: conta-azul-cobranças-charges
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-charge-openapi.yml
- filename: conta-azul-contracts-openapi.yml
  format: yaml
  label: Conta Azul Contratos (Contracts)
  slug: conta-azul-contratos-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-contracts-openapi.yml
- filename: conta-azul-financial-openapi.yml
  format: yaml
  label: Conta Azul Financeiro (Financial)
  slug: conta-azul-financeiro-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-financial-openapi.yml
- filename: conta-azul-inventory-openapi.yml
  format: yaml
  label: Conta Azul Produtos (Inventory)
  slug: conta-azul-produtos-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-inventory-openapi.yml
- filename: conta-azul-proposal-openapi.yml
  format: yaml
  label: Conta Azul Orçamentos (Proposals)
  slug: conta-azul-orçamentos-proposals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-proposal-openapi.yml
- filename: conta-azul-protocol-openapi.yml
  format: yaml
  label: Conta Azul Protocolos (Protocol)
  slug: conta-azul-protocolos-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-protocol-openapi.yml
- filename: conta-azul-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas (Sales)
  slug: conta-azul-vendas-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-sales-openapi.yml
- filename: conta-azul-scheduled-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas Programadas (Scheduled Sales)
  slug: conta-azul-vendas-programadas-scheduled-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-scheduled-sales-openapi.yml
authorization_urls:
- https://auth.contaazul.com/login
description: ''
docs: https://developers.contaazul.com/auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Conta Azul Scopes
name_suffix: OAuth Scopes
note: Conta Azul's Nova API uses a single FIXED scope string on the OAuth2 authorization request. Per the migration guide, requesting this scope grants the developer access to ALL API contexts, so there is no per-resource scope surface to enumerate. The OpenAPI specs do not declare oauth2 scopes (they declare only the resulting bearer scheme); these scopes are captured from the documented authorization flow.
overview: 'Conta Azul publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conta Azul API on a user''s behalf.


  Tokens are issued from https://auth.contaazul.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conta Azul
provider_slug: conta-azul
schemes:
- flows:
  - authorizationUrl: https://auth.contaazul.com/login
    flow: authorizationCode
    tokenUrl: https://auth.contaazul.com/oauth2/token
  name: OAuth2
  source: docs (https://developers.contaazul.com/auth)
scope_count: 3
scope_names:
- openid
- profile
- aws.cognito.signin.user.admin
scopes:
- description: OpenID Connect authentication (identity).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the connected user's profile.
  flows:
  - authorizationCode
  scope: profile
- description: AWS Cognito admin scope — grants full administrative access to all Conta Azul API contexts for the authorizing tenant.
  flows:
  - authorizationCode
  scope: aws.cognito.signin.user.admin
slug: conta-azul-scopes
source_filename: conta-azul-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.contaazul.com/requestingcode + https://developers.contaazul.com/migration\ndocs: https://developers.contaazul.com/auth\nnote: >-\n  Conta Azul's Nova API uses a single FIXED scope string on the OAuth2\n  authorization request. Per the migration guide, requesting this scope grants\n  the developer access to ALL API contexts, so there is no per-resource scope\n  surface to enumerate. The OpenAPI specs do not declare oauth2 scopes (they\n  declare only the resulting bearer scheme); these scopes are captured from the\n  documented authorization flow.\nschemes:\n- name: OAuth2\n  source: docs (https://developers.contaazul.com/auth)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.contaazul.com/login\n    tokenUrl: https://auth.contaazul.com/oauth2/token\nfixed_scope_string: openid profile aws.cognito.signin.user.admin\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\
  \ (identity).\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the connected user's profile.\n  flows: [authorizationCode]\n- scope: aws.cognito.signin.user.admin\n  description: >-\n    AWS Cognito admin scope — grants full administrative access to all Conta\n    Azul API contexts for the authorizing tenant.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/scopes/conta-azul-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Fintech
- Accounting
- ERP
- Brazil
- Small Business
- Financial Management
- Invoicing
- Payments
token_urls:
- https://auth.contaazul.com/oauth2/token
---
