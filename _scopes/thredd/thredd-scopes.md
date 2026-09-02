---
authorization_urls: []
description: ''
docs: https://cardsapidocs.thredd.com/v2.0/docs/get-an-authentication-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Thredd Scopes
name_suffix: OAuth Scopes
note: Thredd uses OAuth2 client-credentials; the access-token audience/scope claims select the backing platform services. Scopes are provisioned per client by the Implementation Manager (not requested via a scope parameter in the token call). The scope set below is taken verbatim from the documented example access-token claims (aud + scope arrays).
overview: 'Thredd publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thredd API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thredd
provider_slug: thredd
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  token_url: https://oauthuat.globalprocessing.net/connect/token
scope_count: 6
scope_names:
- coreapi
- claimsapi
- ctslite
- dalapi
- mdesrttapi
- relayapi
scopes:
- description: Core issuing and card-management platform API (Cards API Hub core).
  flows:
  - clientCredentials
  scope: coreapi
- description: Claims / disputes and chargeback platform service.
  flows:
  - clientCredentials
  scope: claimsapi
- description: Card Transaction System (CTS) transaction data and reporting service.
  flows:
  - clientCredentials
  scope: ctslite
- description: Data access layer service.
  flows:
  - clientCredentials
  scope: dalapi
- description: Mastercard Digital Enablement Service (MDES) real-time tokenisation service for digital wallets.
  flows:
  - clientCredentials
  scope: mdesrttapi
- description: Relay / event-relay service supporting webhooks and notifications.
  flows:
  - clientCredentials
  scope: relayapi
slug: thredd-scopes
source_filename: thredd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://cardsapidocs.thredd.com/docs/get-an-authentication-token\ndocs: https://cardsapidocs.thredd.com/v2.0/docs/get-an-authentication-token\nnote: >-\n  Thredd uses OAuth2 client-credentials; the access-token audience/scope claims\n  select the backing platform services. Scopes are provisioned per client by the\n  Implementation Manager (not requested via a scope parameter in the token call).\n  The scope set below is taken verbatim from the documented example access-token\n  claims (aud + scope arrays).\nschemes:\n  - name: oauth2ClientCredentials\n    flow: clientCredentials\n    token_url: https://oauthuat.globalprocessing.net/connect/token\nscopes:\n  - scope: coreapi\n    description: Core issuing and card-management platform API (Cards API Hub core).\n    flows: [clientCredentials]\n  - scope: claimsapi\n    description: Claims / disputes and chargeback platform service.\n    flows: [clientCredentials]\n  - scope: ctslite\n\
  \    description: Card Transaction System (CTS) transaction data and reporting service.\n    flows: [clientCredentials]\n  - scope: dalapi\n    description: Data access layer service.\n    flows: [clientCredentials]\n  - scope: mdesrttapi\n    description: Mastercard Digital Enablement Service (MDES) real-time tokenisation service for digital wallets.\n    flows: [clientCredentials]\n  - scope: relayapi\n    description: Relay / event-relay service supporting webhooks and notifications.\n    flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thredd/refs/heads/main/scopes/thredd-scopes.yml
summary_line: 6 scopes
tags:
- Payments
- United Kingdom
- Issuer Processor
- Card Issuing
- Payment Processing
- Banking as a Service
- Digital Wallet
- Cross-Border
- Fraud
- Open Banking
- FAPI
token_urls: []
---
