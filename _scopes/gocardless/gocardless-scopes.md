---
api_specs:
- filename: openapi
  format: yaml
  label: GoCardless REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://developer.gocardless.com/api-reference/openapi
authorization_urls: []
description: GoCardless's OAuth surface. The core REST API authenticates with a Bearer access token issued from the dashboard (no OAuth), so the OpenAPI securitySchemes carry no oauth2 scopes and the derive pass finds none. OAuth is used by Partner apps ("Connect with GoCardless") so an integrator can act on behalf of a merchant's GoCardless account. This is the searched fill capturing that Partner OAuth scheme and its single documented scope.
docs: https://developer.gocardless.com/partners/connecting-your-users/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gocardless Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GoCardless publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the GoCardless API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoCardless
provider_slug: gocardless
schemes:
- authorizationUrl: https://connect.gocardless.com/oauth/authorize
  docs: https://developer.gocardless.com/partners/connecting-your-users/
  grant_types:
  - authorization_code
  name: GoCardless Partner OAuth
  notes: Partner apps register a client_id/client_secret and a fixed redirect_uri (must match exactly). The merchant completes the flow and is redirected back with an authorization code, which the partner swaps for an access token scoped to that merchant's account. The same flow exists in sandbox via connect-sandbox.gocardless.com.
  response_type: code
  sandbox_authorizationUrl: https://connect-sandbox.gocardless.com/oauth/authorize
  tokenUrl: https://connect.gocardless.com/oauth/access_token
  token_use: 'Authorization: Bearer <access_token> on subsequent API calls'
  type: oauth2
scope_count: 1
scope_names:
- read_write
scopes:
- description: Full read and write access to the connected merchant's GoCardless account (the scope requested by Partner apps).
  flows: []
  scope: read_write
slug: gocardless-scopes
source_filename: gocardless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nsource: https://developer.gocardless.com/partners/connecting-your-users/\ndocs: https://developer.gocardless.com/partners/connecting-your-users/\ndescription: >-\n  GoCardless's OAuth surface. The core REST API authenticates with a Bearer\n  access token issued from the dashboard (no OAuth), so the OpenAPI\n  securitySchemes carry no oauth2 scopes and the derive pass finds none. OAuth\n  is used by Partner apps (\"Connect with GoCardless\") so an integrator can act\n  on behalf of a merchant's GoCardless account. This is the searched fill\n  capturing that Partner OAuth scheme and its single documented scope.\nschemes:\n  - name: GoCardless Partner OAuth\n    type: oauth2\n    grant_types: [authorization_code]\n    authorizationUrl: https://connect.gocardless.com/oauth/authorize\n    tokenUrl: https://connect.gocardless.com/oauth/access_token\n    sandbox_authorizationUrl: https://connect-sandbox.gocardless.com/oauth/authorize\n  \
  \  response_type: code\n    token_use: 'Authorization: Bearer <access_token> on subsequent API calls'\n    docs: https://developer.gocardless.com/partners/connecting-your-users/\n    notes: >-\n      Partner apps register a client_id/client_secret and a fixed redirect_uri\n      (must match exactly). The merchant completes the flow and is redirected\n      back with an authorization code, which the partner swaps for an access\n      token scoped to that merchant's account. The same flow exists in sandbox\n      via connect-sandbox.gocardless.com.\nscopes:\n  - scope: read_write\n    description: Full read and write access to the connected merchant's GoCardless account (the scope requested by Partner apps).\n    schemes: [GoCardless Partner OAuth]\n    default: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/scopes/gocardless-scopes.yml
summary_line: 1 scope
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscriptions
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
token_urls: []
---
