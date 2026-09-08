---
authorization_urls:
- https://sso.essendant.com/adfs/oauth2/authorize/
- https://login.essendant.com/adfs/oauth2/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Essendant Scopes
name_suffix: OAuth Scopes
note: These are the scopes advertised by Essendant's AD FS OpenID Connect discovery documents. They are the AD FS default set — Essendant has not defined API-specific scopes, because it publishes no API. No scopes/permissions reference page exists on essendant.com. Kept as an honest record of what the discovery document actually advertises.
overview: 'Essendant publishes 9 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Essendant API on a user''s behalf.


  Tokens are issued from https://sso.essendant.com/adfs/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Essendant
provider_slug: essendant
schemes:
- flows:
  - authorizationUrl: https://sso.essendant.com/adfs/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/
  - flow: clientCredentials
    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/
  - deviceAuthorizationUrl: https://sso.essendant.com/adfs/oauth2/devicecode
    flow: deviceCode
    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/
  name: essendant-adfs-sso
  source: well-known/essendant-sso-openid-configuration.json
- flows:
  - authorizationUrl: https://login.essendant.com/adfs/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://login.essendant.com/adfs/oauth2/token/
  name: essendant-adfs-login
  source: well-known/essendant-login-openid-configuration.json
scope_count: 9
scope_names:
- openid
- profile
- email
- allatclaims
- user_impersonation
- aza
- logon_cert
- vpn_cert
- winhello_cert
scopes:
- description: OpenID Connect sign-in; issues an id_token.
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims about the signed-in user.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim for the signed-in user.
  flows:
  - authorizationCode
  scope: email
- description: AD FS scope requesting that all claims be included in the access token.
  flows:
  - authorizationCode
  scope: allatclaims
- description: AD FS delegation scope — act on behalf of the signed-in user.
  flows:
  - authorizationCode
  scope: user_impersonation
- description: AD FS broker/primary-refresh-token scope.
  flows:
  - authorizationCode
  scope: aza
- description: AD FS scope for issuing a logon certificate.
  flows:
  - authorizationCode
  scope: logon_cert
- description: AD FS scope for issuing a VPN certificate.
  flows:
  - authorizationCode
  scope: vpn_cert
- description: AD FS scope for issuing a Windows Hello for Business certificate.
  flows:
  - authorizationCode
  scope: winhello_cert
slug: essendant-scopes
source_filename: essendant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://sso.essendant.com/adfs/.well-known/openid-configuration\nnote: >-\n  These are the scopes advertised by Essendant's AD FS OpenID Connect discovery documents.\n  They are the AD FS default set — Essendant has not defined API-specific scopes, because\n  it publishes no API. No scopes/permissions reference page exists on essendant.com. Kept\n  as an honest record of what the discovery document actually advertises.\nschemes:\n- name: essendant-adfs-sso\n  source: well-known/essendant-sso-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.essendant.com/adfs/oauth2/authorize/\n    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/\n  - flow: clientCredentials\n    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://sso.essendant.com/adfs/oauth2/devicecode\n    tokenUrl: https://sso.essendant.com/adfs/oauth2/token/\n\
  - name: essendant-adfs-login\n  source: well-known/essendant-login-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.essendant.com/adfs/oauth2/authorize/\n    tokenUrl: https://login.essendant.com/adfs/oauth2/token/\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issues an id_token.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: profile\n  description: Profile claims about the signed-in user.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: email\n  description: Email claim for the signed-in user.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: allatclaims\n  description: AD FS scope requesting\
  \ that all claims be included in the access token.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: user_impersonation\n  description: AD FS delegation scope — act on behalf of the signed-in user.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: aza\n  description: AD FS broker/primary-refresh-token scope.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: logon_cert\n  description: AD FS scope for issuing a logon certificate.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: vpn_cert\n  description: AD FS scope for issuing a VPN certificate.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\n- scope: winhello_cert\n  description: AD FS scope for issuing a Windows Hello for Business certificate.\n  flows: [authorizationCode]\n  sources: [well-known/essendant-sso-openid-configuration.json, well-known/essendant-login-openid-configuration.json]\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/essendant/refs/heads/main/scopes/essendant-scopes.yml
summary_line: 9 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Wholesale
- Distribution
- Supply Chain
- Office Supplies
- Fulfillment
- 3PL
- B2B
- EDI
- Ecommerce
- JanSan
- Foodservice
token_urls:
- https://sso.essendant.com/adfs/oauth2/token/
- https://login.essendant.com/adfs/oauth2/token/
---
