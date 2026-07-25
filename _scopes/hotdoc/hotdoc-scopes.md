---
authorization_urls:
- https://www.hotdoc.com.au/oauth/authorize
description: ''
docs: https://www.hotdoc.com.au/.well-known/openid-configuration
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Hotdoc Scopes
name_suffix: OAuth Scopes
note: HotDoc's OpenID Connect discovery document advertises a single OAuth 2.0 scope, "openid". No broader resource/API scope surface (read/write per-resource scopes) is published; the authorization server issues OIDC identity tokens whose claims (practice_name, pms_software, access_level, company) carry the authorization context rather than granular scopes. Additional scopes, if any, are gated behind partner/clinic client registration and are not publicly documented.
overview: 'HotDoc publishes 1 OAuth 2.0 scope via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the HotDoc API on a user''s behalf.


  Tokens are issued from https://www.hotdoc.com.au/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HotDoc
provider_slug: hotdoc
schemes:
- flows:
  - authorizationUrl: https://www.hotdoc.com.au/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.hotdoc.com.au/oauth/token
  - authorizationUrl: https://www.hotdoc.com.au/oauth/authorize
    flow: implicit
  name: HotDocOAuth2
  source: well-known/hotdoc-oauth-authorization-server.json
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication; returns an ID token with the subject and profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: openid
slug: hotdoc-scopes
source_filename: hotdoc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://www.hotdoc.com.au/.well-known/openid-configuration\ndocs: https://www.hotdoc.com.au/.well-known/openid-configuration\nnote: >-\n  HotDoc's OpenID Connect discovery document advertises a single OAuth 2.0 scope,\n  \"openid\". No broader resource/API scope surface (read/write per-resource scopes)\n  is published; the authorization server issues OIDC identity tokens whose claims\n  (practice_name, pms_software, access_level, company) carry the authorization\n  context rather than granular scopes. Additional scopes, if any, are gated behind\n  partner/clinic client registration and are not publicly documented.\nschemes:\n- name: HotDocOAuth2\n  source: well-known/hotdoc-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.hotdoc.com.au/oauth/authorize\n    tokenUrl: https://www.hotdoc.com.au/oauth/token\n  - flow: implicit\n    authorizationUrl: https://www.hotdoc.com.au/oauth/authorize\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token with the subject and profile claims.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/hotdoc-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotdoc/refs/heads/main/scopes/hotdoc-scopes.yml
summary_line: 1 scope · authorizationCode/implicit
tags:
- Healthcare
- Australia
- Patient Engagement
- Online Booking
- Appointment Scheduling
- Telehealth
- Practice Management
- Primary Care
- Digital Health
- e-Prescribing
token_urls:
- https://www.hotdoc.com.au/oauth/token
---
