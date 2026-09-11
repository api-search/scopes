---
authorization_urls:
- https://app.advicepay.com/oauth2/authorize
description: ''
docs: https://docs.advicepay.com/#authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Advicepay Scopes
name_suffix: OAuth Scopes
note: AdvicePay publishes no OpenAPI, so derive-oauth-scopes.py has no spec to read; this file was written from the published OAuth documentation instead. AdvicePay operates OAuth 2.0 but has not (yet) decomposed access into granular scopes — the docs state plainly that "Currently, only 'all' is supported" for the scope parameter on the authorization request. Authorization is therefore all-or-nothing at the token level and is narrowed instead by the role of the authorizing user (admin / advisor / account owner) and by the plan. This is an honest record of a single coarse scope, not a gap in our reading.
overview: 'AdvicePay publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdvicePay API on a user''s behalf.


  Tokens are issued from https://app.advicepay.com/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdvicePay
provider_slug: advicepay
schemes:
- flows:
  - authorizationUrl: https://app.advicepay.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.advicepay.com/oauth2/access_token
  - flow: clientCredentials
    tokenUrl: https://app.advicepay.com/oauth2/access_token
  name: OAuth2
  source: https://docs.advicepay.com/#authentication
scope_count: 1
scope_names:
- all
scopes:
- description: Full access to the AdvicePay public API on behalf of the authorizing user or account owner. The only scope value the authorization endpoint accepts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: all
slug: advicepay-scopes
source_filename: advicepay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://docs.advicepay.com/#oauth-authorization-code-flow\ndocs: https://docs.advicepay.com/#authentication\nnote: >-\n  AdvicePay publishes no OpenAPI, so derive-oauth-scopes.py has no spec to read; this file was\n  written from the published OAuth documentation instead. AdvicePay operates OAuth 2.0 but has\n  not (yet) decomposed access into granular scopes — the docs state plainly that \"Currently, only\n  'all' is supported\" for the scope parameter on the authorization request. Authorization is\n  therefore all-or-nothing at the token level and is narrowed instead by the role of the\n  authorizing user (admin / advisor / account owner) and by the plan. This is an honest record of\n  a single coarse scope, not a gap in our reading.\nschemes:\n- name: OAuth2\n  source: https://docs.advicepay.com/#authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.advicepay.com/oauth2/authorize\n    tokenUrl:\
  \ https://app.advicepay.com/oauth2/access_token\n  - flow: clientCredentials\n    tokenUrl: https://app.advicepay.com/oauth2/access_token\nscopes:\n- scope: all\n  description: >-\n    Full access to the AdvicePay public API on behalf of the authorizing user or account owner.\n    The only scope value the authorization endpoint accepts.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://docs.advicepay.com/#oauth-authorization-code-flow\nscope_granularity: coarse\nscope_count: 1\neffective_authorization:\n  model: role-and-tenant\n  description: >-\n    Because there is one scope, what a token can actually reach is decided by who authorized it.\n    An authorization-code token is bound to a single AdvicePay user and inherits that user's role\n    (admin, advisor, reviewer) and office/firm boundary; a client-credentials token acts as the\n    enterprise account owner across the firm. The /me endpoint is the documented way for an\n    integrator to discover which\
  \ identity and role a token actually carries.\n  discovery_operation: GET /api/public/v1/me\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advicepay/refs/heads/main/scopes/advicepay-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Financial Services
- Payments
- Billing
- Invoicing
- Financial Planning
- Wealth Management
- Subscriptions
- eSignature
- Compliance
- FinTech
token_urls:
- https://app.advicepay.com/oauth2/access_token
---
