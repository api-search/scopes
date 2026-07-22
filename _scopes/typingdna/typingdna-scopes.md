---
api_specs:
- filename: typingdna-authentication-api-openapi-original.json
  format: json
  label: TypingDNA Authentication API
  slug: typingdna-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-authentication-api-openapi-original.json
- filename: typingdna-verify-2fa-openapi.json
  format: json
  label: TypingDNA Verify 2FA API
  slug: typingdna-verify-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-verify-2fa-openapi.json
authorization_urls:
- https://verify.typingdna.com/oidc/auth
description: ''
docs: https://verify.typingdna.com/docs/
flows:
- authorizationCode
- refreshToken
- deviceCode
- jwtBearer
kind: oauth-scopes
layout: scope
method: searched
name: Typingdna Scopes
name_suffix: OAuth Scopes
note: The Authentication API itself is HTTP Basic (apiKey/apiSecret) and has no OAuth scope surface. The scopes below belong to the Verify 2FA OIDC integration, whose live discovery document is captured in well-known/typingdna-verify-openid-configuration.json.
overview: 'TypingDNA publishes 3 OAuth 2.0 scopes via the authorizationCode, refreshToken, deviceCode, and jwtBearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the TypingDNA API on a user''s behalf.


  Tokens are issued from https://verify.typingdna.com/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TypingDNA
provider_slug: typingdna
schemes:
- flows:
  - authorizationUrl: https://verify.typingdna.com/oidc/auth
    flow: authorizationCode
    tokenUrl: https://verify.typingdna.com/oidc/token
  - flow: refreshToken
    tokenUrl: https://verify.typingdna.com/oidc/token
  - flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
  - flow: jwtBearer
    grant: urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://verify.typingdna.com
  name: Verify 2FA OIDC
  source: well-known/typingdna-verify-openid-configuration.json
  type: openIdConnect
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect authentication; returns the id_token (RS256) asserting the typing-biometrics verification.
  flows:
  - authorizationCode
  scope: openid
- description: Release the email claims (email, email_verified) in the id_token/userinfo.
  flows:
  - authorizationCode
  scope: email
- description: Release profile claims (name, given_name, family_name, locale, picture) in the id_token/userinfo.
  flows:
  - authorizationCode
  scope: profile
slug: typingdna-scopes
source_filename: typingdna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://verify.typingdna.com/.well-known/openid-configuration\ndocs: https://verify.typingdna.com/docs/\nnote: >-\n  The Authentication API itself is HTTP Basic (apiKey/apiSecret) and has no\n  OAuth scope surface. The scopes below belong to the Verify 2FA OIDC\n  integration, whose live discovery document is captured in\n  well-known/typingdna-verify-openid-configuration.json.\nschemes:\n  - name: Verify 2FA OIDC\n    type: openIdConnect\n    issuer: https://verify.typingdna.com\n    source: well-known/typingdna-verify-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://verify.typingdna.com/oidc/auth\n        tokenUrl: https://verify.typingdna.com/oidc/token\n      - flow: refreshToken\n        tokenUrl: https://verify.typingdna.com/oidc/token\n      - flow: deviceCode\n        grant: urn:ietf:params:oauth:grant-type:device_code\n      - flow: jwtBearer\n        grant:\
  \ urn:ietf:params:oauth:grant-type:jwt-bearer\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; returns the id_token (RS256) asserting the typing-biometrics verification.\n    flows: [authorizationCode]\n    sources: [well-known/typingdna-verify-openid-configuration.json]\n  - scope: email\n    description: 'Release the email claims (email, email_verified) in the id_token/userinfo.'\n    flows: [authorizationCode]\n    sources: [well-known/typingdna-verify-openid-configuration.json]\n  - scope: profile\n    description: 'Release profile claims (name, given_name, family_name, locale, picture) in the id_token/userinfo.'\n    flows: [authorizationCode]\n    sources: [well-known/typingdna-verify-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/scopes/typingdna-scopes.yml
summary_line: 3 scopes · authorizationCode/refreshToken/deviceCode/jwtBearer
tags:
- Company
- Authentication
- Biometrics
- Typing Biometrics
- Two-Factor Authentication
- Identity
- Security
- Fraud Prevention
token_urls:
- https://verify.typingdna.com/oidc/token
---
