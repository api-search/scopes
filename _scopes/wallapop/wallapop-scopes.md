---
api_specs:
- filename: wallapop-items-openapi-original.yml
  format: yaml
  label: Wallapop Items Connect API
  slug: wallapop-items-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-items-openapi-original.yml
- filename: wallapop-transactions-openapi-original.yml
  format: yaml
  label: Wallapop Transactions Connect API
  slug: wallapop-transactions-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-transactions-openapi-original.yml
- filename: wallapop-webhooks-openapi-original.yml
  format: yaml
  label: Wallapop Webhooks Connect API
  slug: wallapop-webhooks-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-webhooks-openapi-original.yml
authorization_urls:
- https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth
description: ''
docs: https://developers.wallapop.com/pages/api-essentials/auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wallapop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wallapop publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wallapop API on a user''s behalf.


  Tokens are issued from https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wallapop
provider_slug: wallapop
schemes:
- description: The Items Connect API uses OAuth 2.0 Authorization Code flow with a Proof Key for Code Exchange.
  flows:
  - authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token
  name: oAuthWithPKCE
  source: openapi/wallapop-items-openapi-original.yml
- description: The Transactions Connect API uses OAuth 2.0 Authorization Code flow with a Proof Key for Code Exchange.
  flows:
  - authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token
  name: oAuthWithPKCE
  source: openapi/wallapop-transactions-openapi-original.yml
- description: The Webhooks Connect API utilizes the OAuth 2.0 Authorization Code flow with Proof Key for Code Exchange (PKCE) for secure authentication and token exchange.
  flows:
  - authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token
  name: oAuthWithPKCE
  source: openapi/wallapop-webhooks-openapi-original.yml
scope_count: 1
scope_names:
- offline_access
scopes:
- description: Refresh-token capability; the only scope returned on Connect API token responses.
  flows:
  - authorizationCode
  scope: offline_access
slug: wallapop-scopes
source_filename: wallapop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wallapop-items-openapi-original.yml, openapi/wallapop-transactions-openapi-original.yml,\n  openapi/wallapop-webhooks-openapi-original.yml\ndocs: https://developers.wallapop.com/pages/api-essentials/auth\nnotes: >-\n  The Wallapop Connect API does not use granular OAuth scopes: the auth guide\n  states \"Just request the code — no need to set extra OAuth scopes\", and the\n  OpenAPI oauth2 flows declare an empty scopes map. Token responses carry\n  scope \"offline_access\" (refresh-token capability). The Keycloak realm's OIDC\n  discovery (well-known/wallapop-openid-configuration.json) advertises the\n  standard realm scopes listed under realm_scopes_supported; these are\n  identity scopes, not API permission scopes.\nschemes:\n- name: oAuthWithPKCE\n  source: openapi/wallapop-items-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth\n\
  \    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token\n  description: The Items Connect API uses OAuth 2.0 Authorization Code flow with a Proof Key\n    for Code Exchange.\n- name: oAuthWithPKCE\n  source: openapi/wallapop-transactions-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth\n    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token\n  description: The Transactions Connect API uses OAuth 2.0 Authorization Code flow with a Proof\n    Key for Code Exchange.\n- name: oAuthWithPKCE\n  source: openapi/wallapop-webhooks-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/auth\n    tokenUrl: https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token\n  description: The Webhooks\
  \ Connect API utilizes the OAuth 2.0 Authorization Code flow with\n    Proof Key for Code Exchange (PKCE) for secure authentication and token exchange.\nscopes:\n- scope: offline_access\n  description: Refresh-token capability; the only scope returned on Connect API token responses.\n  flows: [authorizationCode]\n  sources: [https://developers.wallapop.com/pages/api-essentials/auth]\nrealm_scopes_supported:\n- openid\n- web-origins\n- roles\n- microprofile-jwt\n- profile\n- address\n- service_account\n- email\n- phone\n- offline_access\n- basic\n- acr\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/scopes/wallapop-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Consumer
- Marketplace
- Ecommerce
- Second-Hand
- Classifieds
- Shipping
- Webhooks
token_urls:
- https://iam.wallapop.com/realms/wallapop-connect/protocol/openid-connect/token
---
