---
authorization_urls:
- https://api.paystand.com/v3/api/v3/oauth/authorize
description: ''
docs: https://developers.paystand.com/reference/access-tokens
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Paystand Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PayStand publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PayStand API on a user''s behalf.


  Tokens are issued from https://api.paystand.com/v3/api/v3/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PayStand
provider_slug: paystand
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token
  - authorizationUrl: https://api.paystand.com/v3/api/v3/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token
  name: oauth2
  source: https://api.paystand.com/.well-known/openid-configuration
scope_count: 1
scope_names:
- auth
scopes:
- description: 'The single scope Paystand advertises in its OpenID Connect discovery document (scopes_supported) and documents on the Access Token page (scope: auth). Access tokens are requested with grant_type=client_credentials.'
  flows:
  - clientCredentials
  - authorizationCode
  scope: auth
slug: paystand-scopes
source_filename: paystand-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.paystand.com/.well-known/openid-configuration\ndocs: https://developers.paystand.com/reference/access-tokens\nschemes:\n- name: oauth2\n  source: https://api.paystand.com/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.paystand.com/v3/api/v3/oauth/authorize\n    tokenUrl: https://api.paystand.com/v3/api/v3/oauth/token\nscopes:\n- scope: auth\n  description: >-\n    The single scope Paystand advertises in its OpenID Connect discovery\n    document (scopes_supported) and documents on the Access Token page\n    (scope: auth). Access tokens are requested with grant_type=client_credentials.\n  flows: [clientCredentials, authorizationCode]\n  sources: [https://api.paystand.com/.well-known/openid-configuration]\nnotes: >-\n  Paystand exposes coarse OAuth scoping — a single\
  \ \"auth\" scope. Fine-grained\n  authorization is enforced by the claims/permissions embedded in the issued\n  token (claims_supported includes roles and permissions), not by OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/scopes/paystand-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Company
- Payments
- B2B Payments
- Accounts Receivable
- Accounts Payable
- Fintech
- Blockchain
- ACH
- Billing
- Checkout
token_urls:
- https://api.paystand.com/v3/api/v3/oauth/token
---
