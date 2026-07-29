---
authorization_urls:
- https://auth.eonnext.com/authorize
description: 'Every scope E.ON Next''s authorization server advertises is a standard OpenID Connect scope or an Auth0 claim-shaped scope. There is no domain scope — no read:meter, no read:usage, no read:billing, no account scope of any kind. That absence is the finding: the authorization server governs identity for the customer account UI, and no energy-data resource server is exposed to third-party clients. Do not read this list as an entitlement model for consumption or billing data; that data has no published API at all.'
docs: ''
flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Eon Next Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'E.ON Next publishes 14 OAuth 2.0 scopes via the authorizationCode, implicit, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the E.ON Next API on a user''s behalf.


  Tokens are issued from https://auth.eonnext.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: E.ON Next
provider_slug: eon-next
schemes:
- flows:
  - authorizationUrl: https://auth.eonnext.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.eonnext.com/oauth/token
  - authorizationUrl: https://auth.eonnext.com/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://auth.eonnext.com/oauth/token
  - deviceAuthorizationUrl: https://auth.eonnext.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.eonnext.com/oauth/token
  issuer: https://auth.eonnext.com/
  name: eon-next-ciam-oidc
  source: well-known/eon-next-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- email_verified
- created_at
- identities
scopes:
- description: Request an ID token — mandatory OIDC scope.
  flows: []
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows: []
  scope: profile
- description: The email claim.
  flows: []
  scope: email
- description: The address claim.
  flows: []
  scope: address
- description: The phone_number claim.
  flows: []
  scope: phone
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Individual claim scope for name.
  flows: []
  scope: name
- description: Individual claim scope for given_name.
  flows: []
  scope: given_name
- description: Individual claim scope for family_name.
  flows: []
  scope: family_name
- description: Individual claim scope for nickname.
  flows: []
  scope: nickname
- description: Individual claim scope for picture.
  flows: []
  scope: picture
- description: Individual claim scope for email_verified.
  flows: []
  scope: email_verified
- description: Individual claim scope for the account creation timestamp.
  flows: []
  scope: created_at
- description: Individual claim scope for linked identity providers.
  flows: []
  scope: identities
slug: eon-next-scopes
source_filename: eon-next-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://auth.eonnext.com/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  E.ON Next publishes no scopes/permissions reference page — no developer portal\n  exists. The scope list below is the scopes_supported array advertised by the\n  authorization server itself, fetched anonymously on 2026-07-27 and saved\n  verbatim at well-known/eon-next-openid-configuration.json.\ndescription: >-\n  Every scope E.ON Next's authorization server advertises is a standard OpenID\n  Connect scope or an Auth0 claim-shaped scope. There is no domain scope — no\n  read:meter, no read:usage, no read:billing, no account scope of any kind. That\n  absence is the finding: the authorization server governs identity for the\n  customer account UI, and no energy-data resource server is exposed to\n  third-party clients. Do not read this list as an entitlement model for\n  consumption or billing data; that data has no published API at all.\n\
  schemes:\n- name: eon-next-ciam-oidc\n  issuer: https://auth.eonnext.com/\n  source: well-known/eon-next-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eonnext.com/authorize\n    tokenUrl: https://auth.eonnext.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.eonnext.com/authorize\n  - flow: clientCredentials\n    tokenUrl: https://auth.eonnext.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.eonnext.com/oauth/device/code\n    tokenUrl: https://auth.eonnext.com/oauth/token\nscopes:\n- {scope: openid, description: 'Request an ID token — mandatory OIDC scope.', standard: 'OpenID Connect Core 1.0'}\n- {scope: profile, description: 'Basic profile claims (name, given_name, family_name, nickname, picture).', standard: 'OpenID Connect Core 1.0'}\n- {scope: email, description: 'The email claim.', standard: 'OpenID Connect Core 1.0'}\n- {scope: address, description: 'The address claim.', standard:\
  \ 'OpenID Connect Core 1.0'}\n- {scope: phone, description: 'The phone_number claim.', standard: 'OpenID Connect Core 1.0'}\n- {scope: offline_access, description: 'Issue a refresh token.', standard: 'OpenID Connect Core 1.0'}\n- {scope: name, description: 'Individual claim scope for name.', standard: 'Auth0 claim scope'}\n- {scope: given_name, description: 'Individual claim scope for given_name.', standard: 'Auth0 claim scope'}\n- {scope: family_name, description: 'Individual claim scope for family_name.', standard: 'Auth0 claim scope'}\n- {scope: nickname, description: 'Individual claim scope for nickname.', standard: 'Auth0 claim scope'}\n- {scope: picture, description: 'Individual claim scope for picture.', standard: 'Auth0 claim scope'}\n- {scope: email_verified, description: 'Individual claim scope for email_verified.', standard: 'Auth0 claim scope'}\n- {scope: created_at, description: 'Individual claim scope for the account creation timestamp.', standard: 'Auth0 claim scope'}\n\
  - {scope: identities, description: 'Individual claim scope for linked identity providers.', standard: 'Auth0 claim scope'}\nscope_count: 14\ndomain_scopes: 0\ndomain_scopes_note: >-\n  No energy, metering, account, tariff, billing or payment scope is advertised.\n  Any such scope would live on a resource-server audience that E.ON Next does not\n  publish.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon-next/refs/heads/main/scopes/eon-next-scopes.yml
summary_line: 14 scopes · authorizationCode/implicit/clientCredentials/deviceCode
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Kraken
- Solar
- EV Charging
- Identity
token_urls:
- https://auth.eonnext.com/oauth/token
---
