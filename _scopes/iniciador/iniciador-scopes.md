---
authorization_urls:
- https://auth.iniciador.com.br/auth
description: ''
docs: https://docs.iniciador.com.br
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Iniciador Scopes
name_suffix: OAuth Scopes
note: Scopes are the Open Finance Brasil standardized API scope set advertised in the provider's OIDC discovery document (scopes_supported). Each maps to an Open Finance Brasil regulated API family.
overview: 'Iniciador publishes 16 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Iniciador API on a user''s behalf.


  Tokens are issued from https://api-mtls.iniciador.com.br/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Iniciador
provider_slug: iniciador
schemes:
- flows:
  - authorizationUrl: https://auth.iniciador.com.br/auth
    flow: authorizationCode
    tokenUrl: https://api-mtls.iniciador.com.br/token
  - flow: clientCredentials
    tokenUrl: https://api-mtls.iniciador.com.br/token
  name: OAuth2
  source: well-known/iniciador-openid-configuration.json
scope_count: 16
scope_names:
- openid
- consents
- resources
- accounts
- credit-cards-accounts
- customers
- loans
- financings
- invoice-financings
- unarranged-accounts-overdraft
- credit-fixed-incomes
- bank-fixed-incomes
- variable-incomes
- treasure-titles
- funds
- exchanges
scopes:
- description: OpenID Connect authentication (subject identity).
  flows: []
  scope: openid
- description: Create and manage Open Finance consent records.
  flows: []
  scope: consents
- description: Access the consented resources list and their availability status.
  flows: []
  scope: resources
- description: Deposit / demand and savings account data.
  flows: []
  scope: accounts
- description: Credit card account data, bills, and transactions.
  flows: []
  scope: credit-cards-accounts
- description: Customer registration / identification data (personal and business).
  flows: []
  scope: customers
- description: Loan contract data.
  flows: []
  scope: loans
- description: Financing contract data.
  flows: []
  scope: financings
- description: Invoice financing (antecipacao de recebiveis) contract data.
  flows: []
  scope: invoice-financings
- description: Unarranged overdraft (cheque especial nao contratado) contract data.
  flows: []
  scope: unarranged-accounts-overdraft
- description: Credit fixed-income investment data (CDB, LCI, LCA, etc.).
  flows: []
  scope: credit-fixed-incomes
- description: Bank fixed-income investment data.
  flows: []
  scope: bank-fixed-incomes
- description: Variable-income investment data (equities, etc.).
  flows: []
  scope: variable-incomes
- description: Treasury title (Tesouro Direto) investment data.
  flows: []
  scope: treasure-titles
- description: Investment fund data.
  flows: []
  scope: funds
- description: Foreign exchange (cambio) operation data.
  flows: []
  scope: exchanges
slug: iniciador-scopes
source_filename: iniciador-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.iniciador.com.br/.well-known/openid-configuration\ndocs: https://docs.iniciador.com.br\nnote: >-\n  Scopes are the Open Finance Brasil standardized API scope set advertised in the\n  provider's OIDC discovery document (scopes_supported). Each maps to an Open\n  Finance Brasil regulated API family.\nschemes:\n- name: OAuth2\n  source: well-known/iniciador-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.iniciador.com.br/auth\n    tokenUrl: https://api-mtls.iniciador.com.br/token\n  - flow: clientCredentials\n    tokenUrl: https://api-mtls.iniciador.com.br/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (subject identity).\n- scope: consents\n  description: Create and manage Open Finance consent records.\n- scope: resources\n  description: Access the consented resources list and their availability status.\n- scope: accounts\n  description:\
  \ Deposit / demand and savings account data.\n- scope: credit-cards-accounts\n  description: Credit card account data, bills, and transactions.\n- scope: customers\n  description: Customer registration / identification data (personal and business).\n- scope: loans\n  description: Loan contract data.\n- scope: financings\n  description: Financing contract data.\n- scope: invoice-financings\n  description: Invoice financing (antecipacao de recebiveis) contract data.\n- scope: unarranged-accounts-overdraft\n  description: Unarranged overdraft (cheque especial nao contratado) contract data.\n- scope: credit-fixed-incomes\n  description: Credit fixed-income investment data (CDB, LCI, LCA, etc.).\n- scope: bank-fixed-incomes\n  description: Bank fixed-income investment data.\n- scope: variable-incomes\n  description: Variable-income investment data (equities, etc.).\n- scope: treasure-titles\n  description: Treasury title (Tesouro Direto) investment data.\n- scope: funds\n  description: Investment\
  \ fund data.\n- scope: exchanges\n  description: Foreign exchange (cambio) operation data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iniciador/refs/heads/main/scopes/iniciador-scopes.yml
summary_line: 16 scopes · authorizationCode/clientCredentials
tags:
- Company
- Fintech
- Open Finance
- Open Banking
- Payments
- Pix
- Brazil
- FAPI
- OAuth
- Financial Services
token_urls:
- https://api-mtls.iniciador.com.br/token
---
