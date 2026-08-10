---
authorization_urls:
- https://auth.liquidinstruments.com/oauth2/authorize
description: ''
docs: https://apis.liquidinstruments.com/cli/login.html
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
- password
kind: oauth-scopes
layout: scope
method: probed
name: Liquid Instruments Scopes
name_suffix: OAuth Scopes
note: There is no OpenAPI declaring oauth2 securitySchemes for Liquid Instruments, so derive-oauth-scopes.py has nothing to read. These scopes were taken verbatim from the live OpenID Connect discovery document at auth.liquidinstruments.com (HTTP 200, application/json, fetched 2026-08-04). Only the standard OIDC scope set is advertised — no product- or resource-specific scopes are published. Liquid Instruments does not publish a scopes/permissions reference page.
overview: 'Liquid Instruments publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Liquid Instruments API on a user''s behalf.


  Tokens are issued from https://auth.liquidinstruments.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Liquid Instruments
provider_slug: liquid-instruments
schemes:
- flows:
  - authorizationUrl: https://auth.liquidinstruments.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.liquidinstruments.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.liquidinstruments.com/oauth2/token
  - deviceAuthorizationUrl: https://auth.liquidinstruments.com/oauth2/device_authorize
    flow: deviceCode
    tokenUrl: https://auth.liquidinstruments.com/oauth2/token
  - authorizationUrl: https://auth.liquidinstruments.com/oauth2/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://auth.liquidinstruments.com/oauth2/token
  issuer: https://auth.liquidinstruments.com
  name: LiquidInstrumentsOIDC
  source: https://auth.liquidinstruments.com/.well-known/openid-configuration
  type: openIdConnect
scope_count: 5
scope_names:
- openid
- offline_access
- email
- phone
- profile
scopes:
- description: Standard OpenID Connect scope — requests an ID token identifying the end user.
  flows: []
  scope: openid
- description: Requests a refresh token so the client can obtain new access tokens without the user being present.
  flows: []
  scope: offline_access
- description: Releases the email and email_verified claims.
  flows: []
  scope: email
- description: Releases the phone_number claim.
  flows: []
  scope: phone
- description: Releases the profile claims (name, given_name, family_name, middle_name, preferred_username, picture, birthdate).
  flows: []
  scope: profile
slug: liquid-instruments-scopes
source_filename: liquid-instruments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://auth.liquidinstruments.com/.well-known/openid-configuration\ndocs: https://apis.liquidinstruments.com/cli/login.html\nnote: 'There is no OpenAPI declaring oauth2 securitySchemes for Liquid Instruments, so\n  derive-oauth-scopes.py has nothing to read. These scopes were taken verbatim from the\n  live OpenID Connect discovery document at auth.liquidinstruments.com (HTTP 200,\n  application/json, fetched 2026-08-04). Only the standard OIDC scope set is advertised\n  — no product- or resource-specific scopes are published. Liquid Instruments does not\n  publish a scopes/permissions reference page.'\nschemes:\n- name: LiquidInstrumentsOIDC\n  type: openIdConnect\n  issuer: https://auth.liquidinstruments.com\n  source: https://auth.liquidinstruments.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.liquidinstruments.com/oauth2/authorize\n    tokenUrl: https://auth.liquidinstruments.com/oauth2/token\n\
  \    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://auth.liquidinstruments.com/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.liquidinstruments.com/oauth2/device_authorize\n    tokenUrl: https://auth.liquidinstruments.com/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://auth.liquidinstruments.com/oauth2/authorize\n  - flow: password\n    tokenUrl: https://auth.liquidinstruments.com/oauth2/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — requests an ID token identifying the end user.\n  standard: true\n  sources: [https://auth.liquidinstruments.com/.well-known/openid-configuration]\n- scope: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens without\n    the user being present.\n  standard: true\n  sources: [https://auth.liquidinstruments.com/.well-known/openid-configuration]\n- scope: email\n  description: Releases the email and email_verified claims.\n\
  \  standard: true\n  sources: [https://auth.liquidinstruments.com/.well-known/openid-configuration]\n- scope: phone\n  description: Releases the phone_number claim.\n  standard: true\n  sources: [https://auth.liquidinstruments.com/.well-known/openid-configuration]\n- scope: profile\n  description: Releases the profile claims (name, given_name, family_name, middle_name,\n    preferred_username, picture, birthdate).\n  standard: true\n  sources: [https://auth.liquidinstruments.com/.well-known/openid-configuration]\nclaims_supported:\n- applicationId\n- at_hash\n- aud\n- authenticationType\n- birthdate\n- c_hash\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- iss\n- jti\n- middle_name\n- name\n- nbf\n- nonce\n- phone_number\n- picture\n- preferred_username\n- roles\n- sub\ngaps:\n- 'No resource-specific scopes are advertised — nothing describes what a token may do\n  against Moku Cloud Compile, licensing, or device features. Authorization appears to be\n  carried\
  \ in a \"roles\" claim rather than in scopes.'\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://auth.liquidinstruments.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-instruments/refs/heads/main/scopes/liquid-instruments-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/deviceCode/implicit/password
tags:
- Company
- Test and Measurement
- Instrumentation
- Hardware
- Oscilloscope
- Spectrum Analyzer
- Data Acquisition
- FPGA
- Photonics
- Scientific Instruments
- Electronics
- Laboratory
token_urls:
- https://auth.liquidinstruments.com/oauth2/token
---
