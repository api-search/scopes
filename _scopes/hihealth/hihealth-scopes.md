---
authorization_urls: []
description: ''
docs: https://partner.getpliant.com/docs/introduction-to-scopes.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hihealth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'hi.health publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the hi.health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: hi.health
provider_slug: hihealth
schemes:
- flow: clientCredentials
  identity_provider: Auth0
  name: OAuth2ClientCredentials
  tokenUrl: https://infinnityprodinternal.eu.auth0.com/oauth/token
scope_count: 3
scope_names:
- sync
- embedded-wallet
- fully-embedded
scopes:
- description: 'Sync scope: read/expense-management integration for pulling card, transaction and receipt data into a partner''s own application (expense management use case).'
  flows: []
  scope: sync
- description: 'Embedded Wallet scope: embed Pliant cards and wallet functionality inside a partner application.'
  flows: []
  scope: embedded-wallet
- description: 'Fully Embedded scope: the deepest integration tier, embedding the full card-issuing and management lifecycle in the partner product.'
  flows: []
  scope: fully-embedded
slug: hihealth-scopes
source_filename: hihealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://partner.getpliant.com/docs/introduction-to-scopes.md\ndocs: https://partner.getpliant.com/docs/introduction-to-scopes.md\nschemes:\n- name: OAuth2ClientCredentials\n  identity_provider: Auth0\n  flow: clientCredentials\n  tokenUrl: https://infinnityprodinternal.eu.auth0.com/oauth/token\nnotes: >-\n  Pliant models partner access as documented \"scopes\" that gate which parts of\n  the CaaS API a partner integration may use (endpoint permissions are documented\n  at /docs/endpoint-permissions). These are integration access tiers rather than\n  free-form OAuth scope strings; the concrete grant is provisioned during partner\n  onboarding.\nscopes:\n- scope: sync\n  description: >-\n    Sync scope: read/expense-management integration for pulling card, transaction\n    and receipt data into a partner's own application (expense management use case).\n  docs: https://partner.getpliant.com/docs/sync-scope.md\n- scope: embedded-wallet\n\
  \  description: >-\n    Embedded Wallet scope: embed Pliant cards and wallet functionality inside a\n    partner application.\n  docs: https://partner.getpliant.com/docs/embedded-wallet-scope.md\n- scope: fully-embedded\n  description: >-\n    Fully Embedded scope: the deepest integration tier, embedding the full\n    card-issuing and management lifecycle in the partner product.\n  docs: https://partner.getpliant.com/docs/fully-embedded-scope.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hihealth/refs/heads/main/scopes/hihealth-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Insurance
- Payments
- Cards
- Fintech
- Health
- Cards-as-a-Service
- Embedded Finance
- Reimbursement
- Claims
token_urls: []
---
