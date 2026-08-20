---
api_specs:
- filename: memo-bank-premium-bank-api-openapi.yml
  format: yaml
  label: Memo Bank Premium Bank API
  slug: memo-bank-premium-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-premium-bank-api-openapi.yml
- filename: memo-bank-marketplace-api-openapi.yml
  format: yaml
  label: Memo Bank Marketplace API
  slug: memo-bank-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-marketplace-api-openapi.yml
- filename: memo-bank-nextgenpsd2-api-openapi.yml
  format: yaml
  label: Memo Bank NextGenPSD2 API
  slug: memo-bank-nextgenpsd2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-nextgenpsd2-api-openapi.yml
authorization_urls:
- https://client.memo.bank/authorize
description: ''
docs: https://docs-marketplace.api.memo.bank/topic/topic-authorization-flow
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Memo Bank Scopes
name_suffix: OAuth Scopes
note: Upgraded from the mechanical derive, which found only the two NextGenPSD2 scopes. Memo Bank operates TWO separate OAuth 2.0 scope systems and only one of them has a published scope list. The NextGenPSD2 scopes (AIS, PIS) are enumerated in that spec's securityScheme. The Marketplace scope system is real and load-bearing - the authorization request takes a space-separated `scope` parameter, the token response returns a granted `scope` string, and Memo Bank tells applicants they must state "a set of scopes your application will have access to" at registration - but NO scope names are published anywhere. The Marketplace authentication page defers to the main API documentation "for the full list of available API endpoints and their required scopes", and the main API documentation does not publish scope names either. That circular reference is recorded below as an unresolved gap rather than filled with guesses.
overview: 'Memo Bank publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Memo Bank API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Memo Bank
provider_slug: memo-bank
schemes:
- flows:
  - authorizationUrl: https://client.memo.bank/authorize
    flow: authorizationCode
    refreshUrl: /oauth2/token
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/memo-bank-nextgenpsd2-api-openapi.yml
  system: nextgenpsd2
- flows:
  - authorizationUrl: https://client.memo.bank/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    refreshUrl: https://api.memo.bank/oauth2/token
    scope_param: space-separated list of requested scopes
    state_param: required, opaque value to maintain state between request and callback
    tokenUrl: https://api.memo.bank/oauth2/token
  name: OAuth2
  source: https://docs-marketplace.api.memo.bank/topic/topic-authorization-flow
  system: marketplace
scope_count: 2
scope_names:
- AIS
- PIS
scopes:
- description: Account Information Service.
  flows:
  - authorizationCode
  scope: AIS
- description: Payment Initiation Service.
  flows:
  - authorizationCode
  scope: PIS
slug: memo-bank-scopes
source_filename: memo-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource:\n- openapi/memo-bank-nextgenpsd2-api-openapi.yml\n- https://docs-marketplace.api.memo.bank/topic/topic-authorization-flow\n- https://docs-marketplace.api.memo.bank/authentication\n- https://docs-marketplace.api.memo.bank/topic/topic-getting-started\ndocs: https://docs-marketplace.api.memo.bank/topic/topic-authorization-flow\nnote: >-\n  Upgraded from the mechanical derive, which found only the two NextGenPSD2 scopes. Memo Bank operates TWO\n  separate OAuth 2.0 scope systems and only one of them has a published scope list. The NextGenPSD2 scopes\n  (AIS, PIS) are enumerated in that spec's securityScheme. The Marketplace scope system is real and\n  load-bearing - the authorization request takes a space-separated `scope` parameter, the token response\n  returns a granted `scope` string, and Memo Bank tells applicants they must state \"a set of scopes your\n  application will have access to\" at registration - but NO scope names\
  \ are published anywhere. The\n  Marketplace authentication page defers to the main API documentation \"for the full list of available API\n  endpoints and their required scopes\", and the main API documentation does not publish scope names either.\n  That circular reference is recorded below as an unresolved gap rather than filled with guesses.\nscope_systems:\n- system: nextgenpsd2\n  published: true\n  scope_count: 2\n  granularity: one scope per PSD2 service role\n- system: marketplace\n  published: false\n  scope_count: 0\n  granularity: unknown\nschemes:\n- name: OAuth2\n  system: nextgenpsd2\n  source: openapi/memo-bank-nextgenpsd2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client.memo.bank/authorize\n    tokenUrl: /oauth2/token\n    refreshUrl: /oauth2/token\n- name: OAuth2\n  system: marketplace\n  source: https://docs-marketplace.api.memo.bank/topic/topic-authorization-flow\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://client.memo.bank/authorize\n    tokenUrl: https://api.memo.bank/oauth2/token\n    refreshUrl: https://api.memo.bank/oauth2/token\n    grant_types:\n    - authorization_code\n    - refresh_token\n    scope_param: space-separated list of requested scopes\n    state_param: required, opaque value to maintain state between request and callback\nscopes:\n- scope: AIS\n  description: Account Information Service.\n  system: nextgenpsd2\n  flows:\n  - authorizationCode\n  operations:\n  - readAccountsList\n  - readAccountDetails\n  - readAccountBalance\n  - readAccountTransactionsList\n  - readAccountTransactionDetails\n  - readCardAccountsList\n  - readCardAccountDetails\n  - readCardAccountBalance\n  - readCardAccountTransactionsList\n  sources:\n  - openapi/memo-bank-nextgenpsd2-api-openapi.yml\n- scope: PIS\n  description: Payment Initiation Service.\n  system: nextgenpsd2\n  flows:\n  - authorizationCode\n  operations:\n  - initiatePayment\n  - getPaymentInformation\n  - getPaymentInitiationStatus\n\
  \  - cancelPayment\n  sources:\n  - openapi/memo-bank-nextgenpsd2-api-openapi.yml\nmarketplace_scopes: []\nmarketplace_scopes_note: >-\n  Deliberately empty. Memo Bank's Marketplace scope names are not published on any public page, and the MCP\n  connector - which uses this same OAuth system - documents its capability boundary in prose (\"can read\n  banking data and attach supporting documents, cannot initiate payments\") rather than as named scopes. The\n  connector's seven tools imply at least a read scope over accounts/IBANs/transactions/attachments and a\n  narrow attachment-write scope, but no scope STRING is published, so none is recorded. Inventing plausible\n  names such as \"accounts:read\" here would be fabrication.\nauthorization_boundaries:\n  workspace_consent: >-\n    Beyond scopes, the user selects which workspace(s) an application or connector may act on during the\n    authorization flow.\n  account_consent: >-\n    Access is further limited to the specific accounts the\
  \ user authorized; requesting resources outside\n    that set returns an error.\n  effective_model: >-\n    Three-dimensional - granted scopes AND authorized workspaces AND authorized accounts must all permit the\n    call. This is a stronger consent model than scopes alone, which is worth noting given the scope names\n    themselves are unpublished.\ngaps:\n- >-\n  No scopes or permissions reference page exists for the Marketplace/MCP OAuth system, despite applicants\n  being required to declare the scopes they need at registration.\n- >-\n  The Marketplace authentication page points at the main API documentation for \"the full list of available\n  API endpoints and their required scopes\", but the main API documentation contains no scope list and its 43\n  operations carry no per-operation OAuth scope requirements - the reference is circular.\n- >-\n  The NextGenPSD2 scopes are coarse: two scopes across 13 operations, with a single PIS scope covering both\n  payment initiation and cancellation.\n\
  - No RFC 8414 authorization-server metadata to expose scopes_supported programmatically.\ncross_links:\n  authentication: authentication/memo-bank-authentication.yml\n  mcp: mcp/memo-bank-mcp.yml\n  well_known: well-known/memo-bank-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/scopes/memo-bank-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fintech Insurtech
- Banking
- Business Banking
- Payments
- SEPA
- SEPA Direct Debit
- Virtual IBAN
- Wire Transfers
- Open Banking
- PSD2
- Berlin Group
- Webhook
- MCP
- France
token_urls:
- /oauth2/token
- https://api.memo.bank/oauth2/token
---
