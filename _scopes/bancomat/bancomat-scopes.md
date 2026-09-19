---
api_specs:
- filename: bancomat-flowpay-api-v1-openapi.yml
  format: yaml
  label: FlowPay API (v1)
  slug: flowpay-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v1-openapi.yml
- filename: bancomat-flowpay-api-v2-openapi.yml
  format: yaml
  label: FlowPay API (v2)
  slug: flowpay-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/openapi/bancomat-flowpay-api-v2-openapi.yml
authorization_urls:
- https://core.flowpay.it/api/openid/authenticate
- /openid/authenticate
description: ''
docs: https://core.flowpay.it/api/openid/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bancomat Scopes
name_suffix: OAuth Scopes
note: 'Two generations of scope vocabulary coexist: v1 uses singular names (account:read, invoice:write, salary:read, bill, pagopa, authorization_intent, reconciliation) and v2 uses plural names (accounts:read, invoices:write, pagopa:read/write, bills:write, ade, wallet:`document_type`). The live OpenID Provider metadata publishes 35 distinct scopes_supported, 15 of which appear in neither contract (added below without descriptions). OpenID Connect scopes openid / profile / email are also supported for user identity.'
overview: 'Bancomat publishes 55 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bancomat API on a user''s behalf.


  Tokens are issued from https://core.flowpay.it/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bancomat
provider_slug: bancomat
schemes:
- description: Autorizzazione oauth ottenuta da terze parti con un authorization flow
  flows:
  - authorizationUrl: https://core.flowpay.it/api/openid/authenticate
    flow: authorizationCode
    tokenUrl: https://core.flowpay.it/api/oauth/token
  name: ThirdPartyAuthorizationCode
  source: openapi/bancomat-flowpay-api-v1-openapi.yml
- description: Autorizzazione oauth ottenuta da terze parti con client credential flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://core.flowpay.it/api/oauth/token
  name: ThirdPartyClientCredential
  source: openapi/bancomat-flowpay-api-v1-openapi.yml
- description: OAuth2 flow
  flows:
  - authorizationUrl: /openid/authenticate
    flow: authorizationCode
    tokenUrl: /oauth/token
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: oAuth2
  source: openapi/bancomat-flowpay-api-v2-openapi.yml
scope_count: 55
scope_names:
- account:read
- account:write
- accounts:read
- accounts:write
- ade
- authorization_code
- authorization_intent
- bill
- bill:write
- bills:read
- bills:write
- business:read
- checkout:read
- construction:read
- construction:write
- constructions:read
- constructions:write
- contacts:read
- fees:read
- invoice:read
- invoice:write
- invoices:read
- invoices:write
- kyc
- openid
- pagopa
- pagopa:read
- pagopa:write
- payment:read
- payments:read
- salary:read
- salary:write
- statistic:read
- transactions:read
- transfer:read
- transfer:write
- transfers:read
- transfers:write
- wallet:`document_type`
- wallet:construction
- profile
- email
- disclaimer
- vatCode
- business
- consumer
- tenant_id
- test_scope
- factoring
- wallet:transfer
- wallet:pagopa
- payment_method:sdd
- payment_method:card
- authentication_level:sca
- track
scopes:
- description: Operazioni di lettura sui conti
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:read
- description: Operazione di modifica sui conti
  flows:
  - clientCredentials
  scope: account:write
- description: Allow to read accounts
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts:read
- description: Allow to mediate accounts creation and open banking consent renewal
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts:write
- description: Allow to interact with Agenzia delle Entrate services
  flows:
  - clientCredentials
  scope: ade
- description: ''
  flows: []
  scope: authorization_code
- description: Creazione di intenti a consensi relativi a risorse di un utente
  flows:
  - clientCredentials
  scope: authorization_intent
- description: Gestione di ricevute
  flows:
  - clientCredentials
  scope: bill
- description: Creazione e gestione di ricevute
  flows:
  - authorizationCode
  scope: bill:write
- description: Allow to read bills
  flows:
  - authorizationCode
  - clientCredentials
  scope: bills:read
- description: Allow to create bills and manage lifecycle
  flows:
  - authorizationCode
  - clientCredentials
  scope: bills:write
- description: Operazioni di lettura sulle informazioni della azienda
  flows:
  - authorizationCode
  - clientCredentials
  scope: business:read
- description: ''
  flows: []
  scope: checkout:read
- description: ''
  flows: []
  scope: construction:read
- description: ''
  flows: []
  scope: construction:write
- description: Allow to read information about construction sites
  flows:
  - authorizationCode
  - clientCredentials
  scope: constructions:read
- description: Allow to create construction sites and manage the lifecycle
  flows:
  - authorizationCode
  - clientCredentials
  scope: constructions:write
- description: Operazioni di lettura sulla rete aziendale
  flows:
  - authorizationCode
  scope: contacts:read
- description: ''
  flows: []
  scope: fees:read
- description: Operazioni di lettura sulle fatture
  flows:
  - authorizationCode
  - clientCredentials
  scope: invoice:read
- description: Operazioni di scrittura sulle fatture
  flows:
  - authorizationCode
  - clientCredentials
  scope: invoice:write
- description: Allow to read invoices
  flows:
  - authorizationCode
  - clientCredentials
  scope: invoices:read
- description: Allow to create invoices and manage lifecycle
  flows:
  - authorizationCode
  - clientCredentials
  scope: invoices:write
- description: ''
  flows: []
  scope: kyc
- description: Allow to read user profile
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: ''
  flows:
  - clientCredentials
  scope: pagopa
- description: Allow to retrieve users' PagoPA payment notices
  flows:
  - authorizationCode
  - clientCredentials
  scope: pagopa:read
- description: Allow to create PagoPA payment notices
  flows:
  - authorizationCode
  - clientCredentials
  scope: pagopa:write
- description: Operazioni di lettura sui pagamenti
  flows:
  - authorizationCode
  - clientCredentials
  scope: payment:read
- description: ''
  flows: []
  scope: payments:read
- description: Operazioni di lettura sulle buste paga
  flows:
  - authorizationCode
  - clientCredentials
  scope: salary:read
- description: Operazioni di scrittura sui salary
  flows:
  - authorizationCode
  - clientCredentials
  scope: salary:write
- description: Lettura dei dati statistici raggruppati
  flows:
  - authorizationCode
  - clientCredentials
  scope: statistic:read
- description: ''
  flows: []
  scope: transactions:read
- description: Operazioni di lettura sui trasferimenti
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfer:read
- description: Operazioni di scrittura sui trasferimenti
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfer:write
- description: Allow to read transfers
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfers:read
- description: Allow to create transfers and manage lifecycle
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfers:write
- description: Allow to manage wallet for the specified use case
  flows:
  - authorizationCode
  - clientCredentials
  scope: wallet:`document_type`
- description: ''
  flows: []
  scope: wallet:construction
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: disclaimer
- description: ''
  flows: []
  scope: vatCode
- description: ''
  flows: []
  scope: business
- description: ''
  flows: []
  scope: consumer
- description: ''
  flows: []
  scope: tenant_id
- description: ''
  flows: []
  scope: test_scope
- description: ''
  flows: []
  scope: factoring
- description: ''
  flows: []
  scope: wallet:transfer
- description: ''
  flows: []
  scope: wallet:pagopa
- description: ''
  flows: []
  scope: payment_method:sdd
- description: ''
  flows: []
  scope: payment_method:card
- description: ''
  flows: []
  scope: authentication_level:sca
- description: ''
  flows: []
  scope: track
slug: bancomat-scopes
source_filename: bancomat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\ndocs: https://core.flowpay.it/api/openid/.well-known/openid-configuration\nsource: openapi/bancomat-flowpay-api-v1-openapi.yml, openapi/bancomat-flowpay-api-v2-openapi.yml; scopes_supported\n  from https://core.flowpay.it/api/openid/.well-known/openid-configuration (200, 2026-09-17)\nnote: 'Two generations of scope vocabulary coexist: v1 uses singular names (account:read, invoice:write, salary:read,\n  bill, pagopa, authorization_intent, reconciliation) and v2 uses plural names (accounts:read, invoices:write, pagopa:read/write,\n  bills:write, ade, wallet:`document_type`). The live OpenID Provider metadata publishes 35 distinct scopes_supported,\n  15 of which appear in neither contract (added below without descriptions). OpenID Connect scopes openid / profile\n  / email are also supported for user identity.'\nscope_count: 55\nschemes:\n- name: ThirdPartyAuthorizationCode\n  source: openapi/bancomat-flowpay-api-v1-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://core.flowpay.it/api/openid/authenticate\n    tokenUrl: https://core.flowpay.it/api/oauth/token\n  description: Autorizzazione oauth ottenuta da terze parti con un authorization flow\n- name: ThirdPartyClientCredential\n  source: openapi/bancomat-flowpay-api-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://core.flowpay.it/api/oauth/token\n  description: Autorizzazione oauth ottenuta da terze parti con client credential flow\n- name: oAuth2\n  source: openapi/bancomat-flowpay-api-v2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /openid/authenticate\n    tokenUrl: /oauth/token\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth2 flow\nscopes:\n- scope: account:read\n  description: Operazioni di lettura sui conti\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n\
  - scope: account:write\n  description: Operazione di modifica sui conti\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: accounts:read\n  description: Allow to read accounts\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: accounts:write\n  description: Allow to mediate accounts creation and open banking consent renewal\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: ade\n  description: Allow to interact with Agenzia delle Entrate services\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: authorization_code\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: authorization_intent\n  description: Creazione di intenti a consensi relativi a risorse di\
  \ un utente\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: bill\n  description: Gestione di ricevute\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: bill:write\n  description: Creazione e gestione di ricevute\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: bills:read\n  description: Allow to read bills\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: bills:write\n  description: Allow to create bills and manage lifecycle\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: business:read\n  description:\
  \ Operazioni di lettura sulle informazioni della azienda\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: checkout:read\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: construction:read\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: construction:write\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: constructions:read\n  description: Allow to read information about construction sites\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: constructions:write\n  description: Allow to create construction sites and manage the lifecycle\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: contacts:read\n  description: Operazioni di lettura sulla rete aziendale\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: fees:read\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: invoice:read\n  description: Operazioni di lettura sulle fatture\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: invoice:write\n  description: Operazioni di scrittura sulle fatture\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: invoices:read\n  description:\
  \ Allow to read invoices\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: invoices:write\n  description: Allow to create invoices and manage lifecycle\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: kyc\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: openid\n  description: Allow to read user profile\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: pagopa\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n- scope: pagopa:read\n  description: Allow to retrieve users' PagoPA payment notices\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n\
  - scope: pagopa:write\n  description: Allow to create PagoPA payment notices\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: payment:read\n  description: Operazioni di lettura sui pagamenti\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: payments:read\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: salary:read\n  description: Operazioni di lettura sulle buste paga\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: salary:write\n  description: Operazioni di scrittura sui salary\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n\
  - scope: statistic:read\n  description: Lettura dei dati statistici raggruppati\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: transactions:read\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: transfer:read\n  description: Operazioni di lettura sui trasferimenti\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: transfer:write\n  description: Operazioni di scrittura sui trasferimenti\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: transfers:read\n  description: Allow to read transfers\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n\
  \  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: transfers:write\n  description: Allow to create transfers and manage lifecycle\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v1-openapi.yml\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: wallet:`document_type`\n  description: Allow to manage wallet for the specified use case\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n- scope: wallet:construction\n  sources:\n  - openapi/bancomat-flowpay-api-v2-openapi.yml\n  - well-known/bancomat-flowpay-openid-configuration.json\n- scope: profile\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: email\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n\
  \  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: disclaimer\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: vatCode\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: business\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: consumer\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n\
  \  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: tenant_id\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: test_scope\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: factoring\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: wallet:transfer\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n\
  \  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: wallet:pagopa\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: payment_method:sdd\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: payment_method:card\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: authentication_level:sca\n  description: null\n\
  \  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n- scope: track\n  description: null\n  flows: []\n  sources:\n  - well-known/bancomat-flowpay-openid-configuration.json\n  note: listed in scopes_supported of the live OpenID Provider metadata but declared in neither OpenAPI; no published\n    description\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bancomat/refs/heads/main/scopes/bancomat-scopes.yml
summary_line: 55 scopes · authorizationCode/clientCredentials
tags:
- ATM
- Banking
- Financial-Services
- Italy
- Mobile Payments
- Payments
- Debit Cards
- Open Banking
- PSD2
- Account Information
- Payment Initiation
- Invoicing
- pagoPA
token_urls:
- https://core.flowpay.it/api/oauth/token
- /oauth/token
---
