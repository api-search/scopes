---
api_specs:
- filename: efi-cobrancas-openapi.yml
  format: yaml
  label: Efí Pay Cobranças API
  slug: efi-cobrancas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-cobrancas-openapi.yml
- filename: efi-pix-openapi.yml
  format: yaml
  label: Efí Pay Pix API
  slug: efi-pix
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pix-openapi.yml
- filename: efi-openfinance-openapi.yml
  format: yaml
  label: Efí Pay Open Finance API
  slug: efi-openfinance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-openfinance-openapi.yml
- filename: efi-contas-openapi.yml
  format: yaml
  label: Efí Pay Contas (Account Opening) API
  slug: efi-contas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-contas-openapi.yml
- filename: efi-pagamentos-openapi.yml
  format: yaml
  label: Efí Pay Pagamentos (Bill Payment) API
  slug: efi-pagamentos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pagamentos-openapi.yml
- filename: efi-extratos-openapi.yml
  format: yaml
  label: Efí Pay Extratos (Statements) API
  slug: efi-extratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-extratos-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Gerencianet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Efí Pay (Gerencianet) publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Efí Pay (Gerencianet) API on a user''s behalf.


  Tokens are issued from https://cobrancas.api.efipay.com.br/v1/authorize.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Efí Pay (Gerencianet)
provider_slug: gerencianet
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://cobrancas.api.efipay.com.br/v1/authorize
  name: oauth2ClientCredentials
  source: openapi/efi-cobrancas-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://abrircontas.api.efipay.com.br/v1/oauth/token
  name: oauth2Contas
  source: openapi/efi-contas-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://extratos.api.efipay.com.br/v1/oauth/token
  name: oauth2Extratos
  source: openapi/efi-extratos-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://openfinance.api.efipay.com.br/v1/oauth/token
  name: oauth2OpenFinance
  source: openapi/efi-openfinance-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://pagarcontas.api.efipay.com.br/v1/oauth/token
  name: oauth2Pagamentos
  source: openapi/efi-pagamentos-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://pix.api.efipay.com.br/oauth/token
  name: oauth2Pix
  source: openapi/efi-pix-openapi.yml
scope_count: 12
scope_names:
- cob.read
- cob.write
- cobv.read
- cobv.write
- gn.balance.read
- openfinance.payments.read
- openfinance.payments.write
- pix.read
- pix.send
- pix.write
- webhook.read
- webhook.write
scopes:
- description: Read immediate charges
  flows:
  - clientCredentials
  scope: cob.read
- description: Create/update immediate charges
  flows:
  - clientCredentials
  scope: cob.write
- description: Read due charges
  flows:
  - clientCredentials
  scope: cobv.read
- description: Create/update due charges
  flows:
  - clientCredentials
  scope: cobv.write
- description: Read account balance
  flows:
  - clientCredentials
  scope: gn.balance.read
- description: Read payment status
  flows:
  - clientCredentials
  scope: openfinance.payments.read
- description: Initiate payments
  flows:
  - clientCredentials
  scope: openfinance.payments.write
- description: Read received Pix
  flows:
  - clientCredentials
  scope: pix.read
- description: Send Pix
  flows:
  - clientCredentials
  scope: pix.send
- description: Manage devolutions
  flows:
  - clientCredentials
  scope: pix.write
- description: Read webhook config
  flows:
  - clientCredentials
  scope: webhook.read
- description: Configure webhooks
  flows:
  - clientCredentials
  scope: webhook.write
slug: gerencianet-scopes
source_filename: gerencianet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/efi-cobrancas-openapi.yml, openapi/efi-contas-openapi.yml, openapi/efi-extratos-openapi.yml,\n  openapi/efi-openfinance-openapi.yml, openapi/efi-pagamentos-openapi.yml, openapi/efi-pix-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/efi-cobrancas-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cobrancas.api.efipay.com.br/v1/authorize\n- name: oauth2Contas\n  source: openapi/efi-contas-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://abrircontas.api.efipay.com.br/v1/oauth/token\n- name: oauth2Extratos\n  source: openapi/efi-extratos-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://extratos.api.efipay.com.br/v1/oauth/token\n- name: oauth2OpenFinance\n  source: openapi/efi-openfinance-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://openfinance.api.efipay.com.br/v1/oauth/token\n- name: oauth2Pagamentos\n\
  \  source: openapi/efi-pagamentos-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://pagarcontas.api.efipay.com.br/v1/oauth/token\n- name: oauth2Pix\n  source: openapi/efi-pix-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://pix.api.efipay.com.br/oauth/token\nscopes:\n- scope: cob.read\n  description: Read immediate charges\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: cob.write\n  description: Create/update immediate charges\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: cobv.read\n  description: Read due charges\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: cobv.write\n  description: Create/update due charges\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: gn.balance.read\n  description: Read account balance\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n\
  - scope: openfinance.payments.read\n  description: Read payment status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-openfinance-openapi.yml\n- scope: openfinance.payments.write\n  description: Initiate payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-openfinance-openapi.yml\n- scope: pix.read\n  description: Read received Pix\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: pix.send\n  description: Send Pix\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: pix.write\n  description: Manage devolutions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: webhook.read\n  description: Read webhook config\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n- scope: webhook.write\n  description: Configure webhooks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/efi-pix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/scopes/gerencianet-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Payments
- Pix
- Boleto
- Subscriptions
- Recurring Billing
- Marketplace
- Split Payments
- Open Finance
- Banking as a Service
- Account Opening
- Bill Payment
- CNAB
- Brazil
- Fintech
token_urls:
- https://cobrancas.api.efipay.com.br/v1/authorize
- https://abrircontas.api.efipay.com.br/v1/oauth/token
- https://extratos.api.efipay.com.br/v1/oauth/token
- https://openfinance.api.efipay.com.br/v1/oauth/token
- https://pagarcontas.api.efipay.com.br/v1/oauth/token
- https://pix.api.efipay.com.br/oauth/token
---
