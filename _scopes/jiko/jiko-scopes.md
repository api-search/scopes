---
authorization_urls:
- https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/authorize
description: ''
docs: https://docs.jiko.io/products/customer-api/guides/oauth/scopes
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Jiko Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jiko publishes 25 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jiko API on a user''s behalf.


  Tokens are issued from https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jiko
provider_slug: jiko
schemes:
- flows:
  - authorizationUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token
  name: CustomerOAuth2
scope_count: 25
scope_names:
- openid
- profile
- email
- phone
- pockets.read
- pockets.write
- transfers.read
- transfers.write
- customer.read
- customer.write
- team.read
- team.write
- onboarding.read
- onboarding.write
- agreements.read
- subscriptions.read
- subscriptions.write
- notifications.read
- notifications.write
- reports.read
- reports.write
- approval_rules.read
- approval_rules.write
- authorization_requests.read
- authorization_requests.write
scopes:
- description: OpenID Connect scope.
  flows: []
  scope: openid
- description: Read information for the current logged-in user.
  flows: []
  scope: profile
- description: Read email for the current logged-in user.
  flows: []
  scope: email
- description: Read phone number for the current logged-in user.
  flows: []
  scope: phone
- description: Read pocket information for a given customer.
  flows: []
  scope: pockets.read
- description: Manage pocket information for a given customer.
  flows: []
  scope: pockets.write
- description: Read transfer and transfer request information for a given customer.
  flows: []
  scope: transfers.read
- description: Create transfers and/or transfer requests.
  flows: []
  scope: transfers.write
- description: Read customer info for a given customer.
  flows: []
  scope: customer.read
- description: Write customer info.
  flows: []
  scope: customer.write
- description: Read team information for a given customer.
  flows: []
  scope: team.read
- description: Manage teams and team members for a given customer.
  flows: []
  scope: team.write
- description: Read onboarding information for a given customer.
  flows: []
  scope: onboarding.read
- description: Manage onboarding information for a given customer.
  flows: []
  scope: onboarding.write
- description: Read agreement information for a given customer.
  flows: []
  scope: agreements.read
- description: Read webhook subscription information (from OIDC discovery; not listed on the scopes doc page).
  flows: []
  scope: subscriptions.read
- description: Manage webhook subscriptions (from OIDC discovery).
  flows: []
  scope: subscriptions.write
- description: Read notifications (from OIDC discovery).
  flows: []
  scope: notifications.read
- description: Manage notifications (from OIDC discovery).
  flows: []
  scope: notifications.write
- description: Read reports (from OIDC discovery).
  flows: []
  scope: reports.read
- description: Generate/manage reports (from OIDC discovery).
  flows: []
  scope: reports.write
- description: Read dual-authorization approval rules (from OIDC discovery).
  flows: []
  scope: approval_rules.read
- description: Manage dual-authorization approval rules (from OIDC discovery).
  flows: []
  scope: approval_rules.write
- description: Read authorization requests (from OIDC discovery).
  flows: []
  scope: authorization_requests.read
- description: Manage authorization requests (from OIDC discovery).
  flows: []
  scope: authorization_requests.write
slug: jiko-scopes
source_filename: jiko-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://authentication-portal.sandbox-api.jikoservices.com/.well-known/openid-configuration\ndocs: https://docs.jiko.io/products/customer-api/guides/oauth/scopes\napi: jiko:jiko-customer-api\nschemes:\n- name: CustomerOAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/authorize\n    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect scope.\n- scope: profile\n  description: Read information for the current logged-in user.\n- scope: email\n  description: Read email for the current logged-in user.\n- scope: phone\n  description: Read phone number for the current logged-in user.\n- scope: pockets.read\n  description: Read pocket information\
  \ for a given customer.\n- scope: pockets.write\n  description: Manage pocket information for a given customer.\n- scope: transfers.read\n  description: Read transfer and transfer request information for a given customer.\n- scope: transfers.write\n  description: Create transfers and/or transfer requests.\n- scope: customer.read\n  description: Read customer info for a given customer.\n- scope: customer.write\n  description: Write customer info.\n- scope: team.read\n  description: Read team information for a given customer.\n- scope: team.write\n  description: Manage teams and team members for a given customer.\n- scope: onboarding.read\n  description: Read onboarding information for a given customer.\n- scope: onboarding.write\n  description: Manage onboarding information for a given customer.\n- scope: agreements.read\n  description: Read agreement information for a given customer.\n- scope: subscriptions.read\n  description: Read webhook subscription information (from OIDC discovery;\
  \ not listed\n    on the scopes doc page).\n- scope: subscriptions.write\n  description: Manage webhook subscriptions (from OIDC discovery).\n- scope: notifications.read\n  description: Read notifications (from OIDC discovery).\n- scope: notifications.write\n  description: Manage notifications (from OIDC discovery).\n- scope: reports.read\n  description: Read reports (from OIDC discovery).\n- scope: reports.write\n  description: Generate/manage reports (from OIDC discovery).\n- scope: approval_rules.read\n  description: Read dual-authorization approval rules (from OIDC discovery).\n- scope: approval_rules.write\n  description: Manage dual-authorization approval rules (from OIDC discovery).\n- scope: authorization_requests.read\n  description: Read authorization requests (from OIDC discovery).\n- scope: authorization_requests.write\n  description: Manage authorization requests (from OIDC discovery).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jiko/refs/heads/main/scopes/jiko-scopes.yml
summary_line: 25 scopes · authorizationCode/clientCredentials
tags:
- Company
- Banking
- Payments
- Treasury
- Embedded Finance
- Fintech
- Cards
- Settlement
- Broker-Dealer
- Banking as a Service
token_urls:
- https://authentication-portal.sandbox-api.jikoservices.com/api/oauth2/token
---
