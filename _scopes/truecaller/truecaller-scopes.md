---
authorization_urls:
- https://oauth-account-noneu.truecaller.com/v1/auth
description: ''
docs: https://docs.truecaller.com/truecaller-sdk/android/latest-oauth-sdk-3.3.0/integration-steps/setting-up-oauth-parameters
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Truecaller Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Truecaller publishes 6 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Truecaller API on a user''s behalf.


  Tokens are issued from https://oauth-account-noneu.truecaller.com/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Truecaller
provider_slug: truecaller
schemes:
- flows:
  - authorizationUrl: https://oauth-account-noneu.truecaller.com/v1/auth
    flow: authorizationCode
    pkce: S256 (required by the SDK integration; code_challenge_methods_supported = [S256])
    revocationUrl: https://oauth-account-noneu.truecaller.com/v1/revoke
    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token
  - flow: refreshToken
    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token
  issuer: https://oauth-account-noneu.truecaller.com
  name: Truecaller OAuth 2.0
  notes: grant_types_supported = [authorization_code, refresh_token]; response_types_supported = [code]; id tokens signed RS256 with per-client JWKS at /.well-known/{clientId}/jwks.json. Scopes requested in-app via TcSdk.getInstance().setOAuthScopes() must also be selected for the project in the developer portal.
scope_count: 6
scope_names:
- openid
- profile
- phone
- email
- address
- offline_access
scopes:
- description: OpenID Connect authentication; required for the userinfo endpoint (422 if missing).
  flows:
  - authorizationCode
  scope: openid
- description: Read the user's Truecaller profile (given_name, family_name, picture, gender).
  flows:
  - authorizationCode
  scope: profile
- description: Read the user's verified phone number, country code and phone_number_verified claim.
  flows:
  - authorizationCode
  scope: phone
- description: Read the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Read the user's address claims (locality, postal_code).
  flows:
  - authorizationCode
  scope: address
- description: Obtain a refresh token for long-lived access.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: truecaller-scopes
source_filename: truecaller-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://oauth-account-noneu.truecaller.com/.well-known/openid-configuration\ndocs: https://docs.truecaller.com/truecaller-sdk/android/latest-oauth-sdk-3.3.0/integration-steps/setting-up-oauth-parameters\nschemes:\n- name: Truecaller OAuth 2.0\n  issuer: https://oauth-account-noneu.truecaller.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-account-noneu.truecaller.com/v1/auth\n    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token\n    revocationUrl: https://oauth-account-noneu.truecaller.com/v1/revoke\n    pkce: S256 (required by the SDK integration; code_challenge_methods_supported = [S256])\n  - flow: refreshToken\n    tokenUrl: https://oauth-account-noneu.truecaller.com/v1/token\n  notes: >-\n    grant_types_supported = [authorization_code, refresh_token];\n    response_types_supported = [code]; id tokens signed RS256 with per-client\n    JWKS at /.well-known/{clientId}/jwks.json.\
  \ Scopes requested in-app via\n    TcSdk.getInstance().setOAuthScopes() must also be selected for the\n    project in the developer portal.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required for the userinfo endpoint (422 if missing).\n  flows: [authorizationCode]\n  sources: [openid-configuration scopes_supported, docs]\n- scope: profile\n  description: Read the user's Truecaller profile (given_name, family_name, picture, gender).\n  flows: [authorizationCode]\n  sources: [openid-configuration scopes_supported, docs]\n- scope: phone\n  description: Read the user's verified phone number, country code and phone_number_verified claim.\n  flows: [authorizationCode]\n  sources: [openid-configuration scopes_supported, docs]\n- scope: email\n  description: Read the user's email address.\n  flows: [authorizationCode]\n  sources: [openid-configuration scopes_supported, docs]\n- scope: address\n  description: Read the user's address claims (locality, postal_code).\n\
  \  flows: [authorizationCode]\n  sources: [openid-configuration scopes_supported, docs]\n- scope: offline_access\n  description: Obtain a refresh token for long-lived access.\n  flows: [authorizationCode, refreshToken]\n  sources: [openid-configuration scopes_supported, docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truecaller/refs/heads/main/scopes/truecaller-scopes.yml
summary_line: 6 scopes · authorizationCode/refreshToken
tags:
- Company
- Consumer
- Caller ID
- Phone Verification
- Identity
- OAuth
- Spam Detection
- Communications
- Mobile SDK
token_urls:
- https://oauth-account-noneu.truecaller.com/v1/token
---
