---
authorization_urls:
- https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize
description: ''
docs: https://docs.safe.security/balbixhelp/docs/provisioning-users-for-sso-enabled-customers
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Balbix Scopes
name_suffix: OAuth Scopes
note: Balbix's REST API v1 is not OAuth-protected — it uses HTTP Basic token exchange plus a Client-API-Key header (see authentication/balbix-authentication.yml). The scopes recorded here belong to the Okta-hosted OpenID Connect authorization server that fronts the Balbix platform web application, harvested anonymously from its published discovery document. They are the standard OIDC scope set; Balbix publishes no custom API scopes.
overview: 'Balbix publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Balbix API on a user''s behalf.


  Tokens are issued from https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Balbix
provider_slug: balbix
schemes:
- flows:
  - authorizationUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token
  issuer: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356
  name: BalbixOkta
  provider: Okta
  source: well-known/balbix-openid-configuration.json
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
scopes:
- description: Required OpenID Connect scope; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Requests the end-user's default profile claims (name, family_name, given_name, preferred_username, picture, locale, updated_at and related).
  flows:
  - authorizationCode
  scope: profile
- description: Requests the email and email_verified claims.
  flows: []
  scope: email
- description: Requests the address claim.
  flows: []
  scope: address
- description: Requests the phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Requests a refresh token so the client can obtain new access tokens without user interaction.
  flows: []
  scope: offline_access
- description: Okta device single sign-on scope; issues a device secret for native SSO across applications on the same device.
  flows: []
  scope: device_sso
slug: balbix-scopes
source_filename: balbix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/.well-known/openid-configuration\ndocs: https://docs.safe.security/balbixhelp/docs/provisioning-users-for-sso-enabled-customers\nnote: Balbix's REST API v1 is not OAuth-protected — it uses HTTP Basic token exchange\n  plus a Client-API-Key header (see authentication/balbix-authentication.yml). The\n  scopes recorded here belong to the Okta-hosted OpenID Connect authorization server\n  that fronts the Balbix platform web application, harvested anonymously from its\n  published discovery document. They are the standard OIDC scope set; Balbix publishes\n  no custom API scopes.\nschemes:\n- name: BalbixOkta\n  provider: Okta\n  issuer: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356\n  source: well-known/balbix-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/authorize\n    tokenUrl:\
  \ https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID token.\n  standard: OpenID Connect Core 1.0\n  requested_by_app: true\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/balbix-openid-configuration.json\n- scope: profile\n  description: Requests the end-user's default profile claims (name, family_name,\n    given_name, preferred_username, picture, locale, updated_at and related).\n  standard: OpenID Connect Core 1.0\n  requested_by_app: true\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/balbix-openid-configuration.json\n- scope: email\n  description: Requests the email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  requested_by_app: false\n  sources:\n  - well-known/balbix-openid-configuration.json\n- scope: address\n  description: Requests the address claim.\n  standard: OpenID Connect Core 1.0\n  requested_by_app: false\n  sources:\n  - well-known/balbix-openid-configuration.json\n\
  - scope: phone\n  description: Requests the phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0\n  requested_by_app: false\n  sources:\n  - well-known/balbix-openid-configuration.json\n- scope: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens\n    without user interaction.\n  standard: OpenID Connect Core 1.0\n  requested_by_app: false\n  sources:\n  - well-known/balbix-openid-configuration.json\n- scope: device_sso\n  description: Okta device single sign-on scope; issues a device secret for native\n    SSO across applications on the same device.\n  standard: Okta extension\n  requested_by_app: false\n  sources:\n  - well-known/balbix-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balbix/refs/heads/main/scopes/balbix-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Cybersecurity
- Security
- Risk Management
- Vulnerability Management
- Exposure Management
- Asset Management
- Cyber Asset Attack Surface Management
- Continuous Threat Exposure Management
- Cyber Risk Quantification
- Application Security
token_urls:
- https://login.balbix.net/oauth2/aus9g844oA86yTqSo356/v1/token
---
