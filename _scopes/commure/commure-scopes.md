---
api_specs:
- filename: commure-auth-api-openapi.yml
  format: yaml
  label: Commure Auth API
  slug: commure-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/openapi/commure-auth-api-openapi.yml
- filename: commure-fhir-api-openapi.yml
  format: yaml
  label: Commure FHIR API
  slug: commure-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/openapi/commure-fhir-api-openapi.yml
authorization_urls:
- https://api-{tenant-id}.developer.commure.com/auth/authorize
description: ''
docs: https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Commure Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Commure publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Commure API on a user''s behalf.


  Tokens are issued from https://api-{tenant-id}.developer.commure.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Commure
provider_slug: commure
schemes:
- description: OpenID Connect / SMART App Launch. Supports the authorization code (with PKCE), implicit, hybrid, client credentials and refresh token grants.
  flows:
  - authorizationUrl: https://api-{tenant-id}.developer.commure.com/auth/authorize
    flow: authorizationCode
    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token
  - flow: clientCredentials
    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token
  name: SMARTonFHIR
  source: openapi/commure-fhir-openapi.yml
scope_count: 5
scope_names:
- email
- launch
- offline_access
- openid
- profile
scopes:
- description: OpenID Connect email claim for the authenticated user.
  flows:
  - authorizationCode
  scope: email
- description: SMART EHR launch context.
  flows:
  - authorizationCode
  scope: launch
- description: Request a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims for the authenticated user.
  flows:
  - authorizationCode
  scope: profile
slug: commure-scopes
source_filename: commure-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: openapi/commure-fhir-openapi.yml\ndocs: https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\nalso_probed:\n- https://accounts.commure.com/oauth2/default/.well-known/openid-configuration\n- https://accounts.commure.com/.well-known/oauth-authorization-server\nschemes:\n- name: SMARTonFHIR\n  source: openapi/commure-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-{tenant-id}.developer.commure.com/auth/authorize\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n  - flow: clientCredentials\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n  description: OpenID Connect / SMART App Launch. Supports the authorization code (with PKCE),\n    implicit, hybrid, client credentials and refresh token grants.\nscopes:\n- scope: email\n  description: OpenID Connect email claim for the authenticated user.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/commure-fhir-openapi.yml\n- scope: launch\n  description: SMART EHR launch context.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/commure-fhir-openapi.yml\n- scope: offline_access\n  description: Request a refresh token for long-lived access.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/commure-fhir-openapi.yml\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/commure-fhir-openapi.yml\n- scope: profile\n  description: OpenID Connect profile claims for the authenticated user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/commure-fhir-openapi.yml\nidentity_provider_scopes:\n  scope_note: >-\n    These scopes are advertised anonymously by Commure's LIVE identity host accounts.commure.com\n    (an Okta Customer Identity org on Commure's own domain). They govern sign-in to Commure's\n    product estate, NOT the FHIR API above - keep the two\
  \ sets separate. Recorded because they are\n    the only Commure OAuth scopes readable from a live, machine-readable document today.\n  method: probed\n  probed: '2026-08-15'\n  authorization_servers:\n  - issuer: https://accounts.commure.com/oauth2/default\n    kind: custom\n    source: well-known/commure-accounts-default-openid-configuration.json\n    commure_configured: true\n    scopes:\n    - scope: default\n      description: Default access scope on Commure's custom authorization server.\n      standard: false\n    - scope: interclient_access\n      description: >-\n        Commure-defined scope; the name indicates cross-client/service access between Commure\n        applications. Commure publishes no description of it.\n      standard: false\n    - scope: device_sso\n      description: Okta device-level single sign-on, enabled on this authorization server.\n      standard: false\n    - scope: groups\n      description: Group memberships of the authenticated user, returned as a claim.\n\
  \      standard: false\n    - scope: openid\n      description: OpenID Connect authentication; returns an ID token.\n      standard: true\n    - scope: profile\n      description: OpenID Connect profile claims.\n      standard: true\n    - scope: email\n      description: OpenID Connect email claim.\n      standard: true\n    - scope: address\n      description: OpenID Connect address claim.\n      standard: true\n    - scope: phone\n      description: OpenID Connect phone_number claim.\n      standard: true\n    - scope: offline_access\n      description: Request a refresh token.\n      standard: true\n  - issuer: https://accounts.commure.com\n    kind: org\n    source: well-known/commure-accounts-oauth-authorization-server.json\n    commure_configured: false\n    scopes_summary: >-\n      Advertises 7 OIDC scopes (openid, email, profile, address, phone, offline_access, groups)\n      plus 78 okta.* management scopes (okta.users.*, okta.groups.*, okta.apps.*, okta.policies.*,\n      okta.logs.read,\
  \ ...). The okta.* set is Okta's own platform management API, identical in\n      every Okta org, and is NOT enumerated here because it says nothing about Commure - see the\n      verbatim document for the full list.\n    okta_platform_scope_count: 78\n    oidc_scope_count: 7\nx-searched:\n  fetched: '2026-08-15'\n  previous: '2026-07-31'\n  sources:\n  - https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\n  - postman/commure-fhir-api-collection.json\n  findings:\n  - Commure publishes no standalone scopes/permissions reference page. The only scope guidance\n    on the public surface is in the \"Commure FHIR API\" collection description, which documents\n    the starter scope set `openid email` against client id `smart_hello_world`.\n  - Commure's authorize endpoint documents the SMART EHR launch and standalone launch sequences,\n    so SMART App Launch resource scopes (patient/*.rs, user/*.rs, system/*.rs) are expected to\n    apply. Commure does NOT enumerate\
  \ them publicly - they are advertised per tenant in\n    /api/v1/r4/.well-known/smart-configuration (`scopes_supported`), which no reachable host\n    currently serves. No SMART resource scopes are asserted here rather than guessing them.\n  - The clientCredentials flow declares no scopes in the published contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/scopes/commure-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- United States
- Clinical AI
- Ambient AI
- Revenue Cycle Management
- FHIR
- SMART on FHIR
- Interoperability
- EHR
- Remote Monitoring
- Health System
- Terminology Services
token_urls:
- https://api-{tenant-id}.developer.commure.com/auth/token
---
