---
api_specs:
- filename: hku-identity-openapi.yml
  format: yaml
  label: HKU AD FS OAuth 2.0 / OpenID Connect Issuer
  slug: adfs-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-identity-openapi.yml
authorization_urls:
- https://adfs.hku.hk/adfs/oauth2/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Hku Scopes
name_suffix: OAuth Scopes
note: Scope strings are read verbatim from scopes_supported in HKU's live OpenID Connect discovery document on its own host. Descriptions are ours. These are the scopes the HKU AD FS issuer advertises to relying parties; HKU publishes no scope documentation of its own, and the HKU ITS API developer portal (developer.hku.hk) does not expose its API scopes without institutional sign-in.
overview: 'University of Hong Kong publishes 9 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Hong Kong API on a user''s behalf.


  Tokens are issued from https://adfs.hku.hk/adfs/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Hong Kong
provider_slug: hku
schemes:
- flows:
  - authorizationUrl: https://adfs.hku.hk/adfs/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  - flow: clientCredentials
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  - deviceAuthorizationUrl: https://adfs.hku.hk/adfs/oauth2/devicecode
    flow: deviceCode
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  issuer: https://adfs.hku.hk/adfs
  name: hku-adfs-oidc
  source: https://adfs.hku.hk/adfs/.well-known/openid-configuration
scope_count: 9
scope_names:
- openid
- profile
- email
- allatclaims
- aza
- user_impersonation
- logon_cert
- winhello_cert
- vpn_cert
scopes:
- description: Standard OpenID Connect scope — issues an ID token for the signed-in HKU account.
  flows:
  - authorizationCode
  - clientCredentials
  - deviceCode
  scope: openid
- description: Releases profile claims (unique_name, upn) about the signed-in account.
  flows:
  - authorizationCode
  scope: profile
- description: Releases the account's email claim.
  flows:
  - authorizationCode
  scope: email
- description: AD FS scope that copies all claims from the underlying authentication into the issued token.
  flows:
  - authorizationCode
  scope: allatclaims
- description: Microsoft broker scope used for primary refresh tokens on managed devices.
  flows:
  - authorizationCode
  scope: aza
- description: Allows a relying party to act on behalf of the signed-in user.
  flows:
  - authorizationCode
  scope: user_impersonation
- description: Requests a logon certificate for certificate-based authentication.
  flows:
  - authorizationCode
  scope: logon_cert
- description: Requests a Windows Hello for Business certificate.
  flows:
  - authorizationCode
  scope: winhello_cert
- description: Requests a VPN client certificate.
  flows:
  - authorizationCode
  scope: vpn_cert
slug: hku-scopes
source_filename: hku-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://adfs.hku.hk/adfs/.well-known/openid-configuration\nx-operator: institution\nnote: >-\n  Scope strings are read verbatim from scopes_supported in HKU's live OpenID Connect discovery\n  document on its own host. Descriptions are ours. These are the scopes the HKU AD FS issuer\n  advertises to relying parties; HKU publishes no scope documentation of its own, and the HKU ITS\n  API developer portal (developer.hku.hk) does not expose its API scopes without institutional\n  sign-in.\nschemes:\n- name: hku-adfs-oidc\n  source: https://adfs.hku.hk/adfs/.well-known/openid-configuration\n  issuer: https://adfs.hku.hk/adfs\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://adfs.hku.hk/adfs/oauth2/authorize/\n    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\n  - flow: clientCredentials\n    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://adfs.hku.hk/adfs/oauth2/devicecode\n\
  \    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — issues an ID token for the signed-in HKU account.\n  flows: [authorizationCode, clientCredentials, deviceCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: profile\n  description: Releases profile claims (unique_name, upn) about the signed-in account.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: email\n  description: Releases the account's email claim.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: allatclaims\n  description: AD FS scope that copies all claims from the underlying authentication into the issued token.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: aza\n  description: Microsoft broker scope used for primary refresh tokens on managed devices.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: user_impersonation\n  description: Allows a relying party to act on behalf of the signed-in user.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: logon_cert\n  description: Requests a logon certificate for certificate-based authentication.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: winhello_cert\n  description: Requests a Windows Hello for Business certificate.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\n- scope: vpn_cert\n  description: Requests a VPN client certificate.\n  flows: [authorizationCode]\n  sources: [well-known/hku-adfs-openid-configuration.json]\nclaims:\n  supported: [aud, iss, iat, exp, auth_time, nonce, at_hash, c_hash, sub, upn, unique_name, pwd_url, pwd_exp, mfa_auth_time, sid, nbf]\n  source: https://adfs.hku.hk/adfs/.well-known/openid-configuration\n\
  samlAttributesReleased:\n  note: >-\n    The Shibboleth IdP at hkafidp.hku.hk declares the attributes it releases in its SAML metadata.\n    They are catalogued in vocabulary/hku-identity-attributes.yml.\n  source: https://hkafidp.hku.hk/idp/shibboleth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/scopes/hku-scopes.yml
summary_line: 9 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Education
- Higher Education
- University
- Hong Kong
- Identity Federation
- Single Sign-On
- Research Data
- Open Access
- Artificial Intelligence
- Research Computing
token_urls:
- https://adfs.hku.hk/adfs/oauth2/token/
---
