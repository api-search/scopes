---
authorization_urls:
- https://auth.cccis.com/oauth2/v1/authorize
- https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ccc Intelligent Solutions Scopes
name_suffix: OAuth Scopes
note: CCC publishes no OpenAPI, so no oauth2 scope map could be derived from a spec. These scopes are read verbatim from the two anonymously readable Okta discovery documents at auth.cccis.com plus the scope observed on the live CCC Connect authorization request. They are identity/portal scopes - CCC does NOT publish any resource scopes for the api.cccis.com gateway or for CCC Secure Share; those are issued privately after contract/CIECA gating.
overview: 'CCC Intelligent Solutions publishes 9 OAuth 2.0 scopes via the authorizationCode, implicit, deviceCode, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CCC Intelligent Solutions API on a user''s behalf.


  Tokens are issued from https://auth.cccis.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CCC Intelligent Solutions
provider_slug: ccc-intelligent-solutions
schemes:
- flows:
  - authorizationUrl: https://auth.cccis.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cccis.com/oauth2/v1/token
  - authorizationUrl: https://auth.cccis.com/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://auth.cccis.com/oauth2/v1/device/authorize
    flow: deviceCode
  - flow: clientCredentials
    note: advertised in the RFC 8414 metadata only; no public client registration
    tokenUrl: https://auth.cccis.com/oauth2/v1/token
  name: CCCOktaOrgAuthorizationServer
  source: well-known/ccc-intelligent-solutions-openid-configuration.json
- flows:
  - authorizationUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/token
  name: CCCOktaConnectAuthorizationServer
  source: well-known/ccc-intelligent-solutions-connect-openid-configuration.json
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
- device_sso
- connect:portal
scopes:
- description: OpenID Connect - request an ID token.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Basic profile claims for the authenticated CCC user.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Email address claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Address claim.
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: Phone number claim.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Issue a refresh token.
  flows:
  - authorizationCode
  scope: offline_access
- description: Okta group membership claim - the group grants that map a CCC user to their entitlements.
  flows:
  - authorizationCode
  - implicit
  scope: groups
- description: Native SSO / device secret exchange on the CCC Connect authorization server.
  flows:
  - authorizationCode
  scope: device_sso
- description: Access to the CCC Connect customer/partner portal. Observed on the live authorization-code + PKCE request issued by connect.cccis.com.
  flows:
  - authorizationCode
  scope: connect:portal
slug: ccc-intelligent-solutions-scopes
source_filename: ccc-intelligent-solutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cccis.com/.well-known/openid-configuration\nnote: |\n  CCC publishes no OpenAPI, so no oauth2 scope map could be derived from a spec.\n  These scopes are read verbatim from the two anonymously readable Okta\n  discovery documents at auth.cccis.com plus the scope observed on the live\n  CCC Connect authorization request. They are identity/portal scopes - CCC does\n  NOT publish any resource scopes for the api.cccis.com gateway or for CCC\n  Secure Share; those are issued privately after contract/CIECA gating.\nschemes:\n- name: CCCOktaOrgAuthorizationServer\n  source: well-known/ccc-intelligent-solutions-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cccis.com/oauth2/v1/authorize\n    tokenUrl: https://auth.cccis.com/oauth2/v1/token\n  - flow: implicit\n    authorizationUrl: https://auth.cccis.com/oauth2/v1/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl:\
  \ https://auth.cccis.com/oauth2/v1/device/authorize\n  - flow: clientCredentials\n    tokenUrl: https://auth.cccis.com/oauth2/v1/token\n    note: advertised in the RFC 8414 metadata only; no public client registration\n- name: CCCOktaConnectAuthorizationServer\n  source: well-known/ccc-intelligent-solutions-connect-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/authorize\n    tokenUrl: https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/token\nscopes:\n- scope: openid\n  description: OpenID Connect - request an ID token.\n  flows: [authorizationCode, implicit]\n  sources: [org, connect]\n- scope: profile\n  description: Basic profile claims for the authenticated CCC user.\n  flows: [authorizationCode, implicit]\n  sources: [org, connect]\n- scope: email\n  description: Email address claim.\n  flows: [authorizationCode, implicit]\n  sources: [org, connect]\n- scope: address\n  description: Address\
  \ claim.\n  flows: [authorizationCode, implicit]\n  sources: [org, connect]\n- scope: phone\n  description: Phone number claim.\n  flows: [authorizationCode, implicit]\n  sources: [org, connect]\n- scope: offline_access\n  description: Issue a refresh token.\n  flows: [authorizationCode]\n  sources: [org, connect]\n- scope: groups\n  description: Okta group membership claim - the group grants that map a CCC user\n    to their entitlements.\n  flows: [authorizationCode, implicit]\n  sources: [org]\n- scope: device_sso\n  description: Native SSO / device secret exchange on the CCC Connect authorization\n    server.\n  flows: [authorizationCode]\n  sources: [connect]\n- scope: 'connect:portal'\n  description: Access to the CCC Connect customer/partner portal. Observed on the\n    live authorization-code + PKCE request issued by connect.cccis.com.\n  flows: [authorizationCode]\n  sources: [observed]\nplatform_scopes:\n  note: |\n    The org authorization server also advertises the full Okta\
  \ management scope\n    set (okta.users.*, okta.groups.*, okta.apps.*, okta.logs.read, and ~70 more).\n    These are Okta platform-administration scopes exposed by every Okta org, not\n    CCC product scopes, and they are recorded here only so a future round does\n    not mistake them for a CCC API surface.\n  count: 77\n  prefix: okta.\ngaps:\n- No resource scopes are published for the api.cccis.com production gateway.\n- No scopes are published for CCC Secure Share; access is per-app and per-BMS\n  message type, assigned by CCC at registration review (\"CCC assigns the\n  appropriate BMS message for each registered app based on business purpose\").\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccc-intelligent-solutions/refs/heads/main/scopes/ccc-intelligent-solutions-scopes.yml
summary_line: 9 scopes · authorizationCode/implicit/deviceCode/clientCredentials
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Auto Physical Damage
- Collision Repair
- Insurtech
- Claims Technology
- CIECA
- Partner Gated
- Authentication
- OpenID Connect
token_urls:
- https://auth.cccis.com/oauth2/v1/token
- https://auth.cccis.com/oauth2/aus294ajl2Qs1RgY24x7/v1/token
---
