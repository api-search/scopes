---
authorization_urls:
- https://cms-login.extu.com/authorize
- https://pexp-login.extu.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Affiniti Scopes
name_suffix: OAuth Scopes
note: Both Auth0 tenants advertise the identical set, and every entry is an OpenID Connect standard scope or standard claim exposed as a scope. There is NO product/API scope here — no campaigns:read, no partners:write — because Affiniti/Extu publishes no API for a third party to request scopes against. Recorded because it is what the provider actually serves; do not read it as a developer permissions model.
overview: 'Affiniti publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Affiniti API on a user''s behalf.


  Tokens are issued from https://cms-login.extu.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Affiniti
provider_slug: affiniti
schemes:
- flows:
  - authorizationUrl: https://cms-login.extu.com/authorize
    flow: authorizationCode
    tokenUrl: https://cms-login.extu.com/oauth/token
  name: extu-cms-auth0
  source: well-known/affiniti-cms-login-openid-configuration.json
- flows:
  - authorizationUrl: https://pexp-login.extu.com/authorize
    flow: authorizationCode
    tokenUrl: https://pexp-login.extu.com/oauth/token
  name: extu-pexp-auth0
  source: well-known/affiniti-pexp-login-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Issue a refresh token
  flows: []
  scope: offline_access
- description: Full name claim
  flows: []
  scope: name
- description: Given name claim
  flows: []
  scope: given_name
- description: Family name claim
  flows: []
  scope: family_name
- description: Nickname claim
  flows: []
  scope: nickname
- description: Email address claim
  flows: []
  scope: email
- description: Email verification status claim
  flows: []
  scope: email_verified
- description: Profile picture claim
  flows: []
  scope: picture
- description: Account creation timestamp claim
  flows: []
  scope: created_at
- description: Linked identity providers (Auth0 extension)
  flows: []
  scope: identities
- description: Phone number claim
  flows: []
  scope: phone
- description: Address claim
  flows: []
  scope: address
slug: affiniti-scopes
source_filename: affiniti-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  scopes_supported in https://cms-login.extu.com/.well-known/openid-configuration and\n  https://pexp-login.extu.com/.well-known/openid-configuration\nnote: >-\n  Both Auth0 tenants advertise the identical set, and every entry is an OpenID Connect standard\n  scope or standard claim exposed as a scope. There is NO product/API scope here — no\n  campaigns:read, no partners:write — because Affiniti/Extu publishes no API for a third party to\n  request scopes against. Recorded because it is what the provider actually serves; do not read it\n  as a developer permissions model.\ndocs: null\nschemes:\n- name: extu-cms-auth0\n  source: well-known/affiniti-cms-login-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cms-login.extu.com/authorize\n    tokenUrl: https://cms-login.extu.com/oauth/token\n- name: extu-pexp-auth0\n  source: well-known/affiniti-pexp-login-openid-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pexp-login.extu.com/authorize\n    tokenUrl: https://pexp-login.extu.com/oauth/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication, standard: true}\n- {scope: profile, description: Basic profile claims, standard: true}\n- {scope: offline_access, description: Issue a refresh token, standard: true}\n- {scope: name, description: Full name claim, standard: true}\n- {scope: given_name, description: Given name claim, standard: true}\n- {scope: family_name, description: Family name claim, standard: true}\n- {scope: nickname, description: Nickname claim, standard: true}\n- {scope: email, description: Email address claim, standard: true}\n- {scope: email_verified, description: Email verification status claim, standard: true}\n- {scope: picture, description: Profile picture claim, standard: true}\n- {scope: created_at, description: Account creation timestamp claim, standard: true}\n- {scope: identities,\
  \ description: Linked identity providers (Auth0 extension), standard: false}\n- {scope: phone, description: Phone number claim, standard: true}\n- {scope: address, description: Address claim, standard: true}\nscope_count: 14\nproduct_scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affiniti/refs/heads/main/scopes/affiniti-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Channel Marketing
- Marketing Automation
- Through-Channel Marketing
- Partner Marketing
- Incentives
- Loyalty
- Rebates
- Rewards
- B2B SaaS
token_urls:
- https://cms-login.extu.com/oauth/token
- https://pexp-login.extu.com/oauth/token
---
