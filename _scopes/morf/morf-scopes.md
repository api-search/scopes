---
authorization_urls:
- https://dashboard.morf.health/authorize
description: ''
docs: https://docs.morf.health/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Morf Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Morf publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Morf API on a user''s behalf.


  Tokens are issued from https://auth.morf.health/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Morf
provider_slug: morf
schemes:
- flows:
  - authorizationUrl: https://dashboard.morf.health/authorize
    flow: authorizationCode
    tokenUrl: https://auth.morf.health/v1/oauth2/token
  name: OAuth2
  source: well-known/morf-openid-configuration.json
scope_count: 6
scope_names:
- openid
- profile
- email
- phone
- offline_access
- full_access
scopes:
- description: OpenID Connect sign-in; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the end user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the end user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the end user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Issue a refresh token for long-lived, offline API access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Full access scope advertised by the OpenID Connect discovery document (scopes_supported). Grants broad access to the Morf API.
  flows:
  - authorizationCode
  scope: full_access
slug: morf-scopes
source_filename: morf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.morf.health/.well-known/openid-configuration\ndocs: https://docs.morf.health/\nschemes:\n- name: OAuth2\n  source: well-known/morf-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.morf.health/authorize\n    tokenUrl: https://auth.morf.health/v1/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; returns an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/morf-openid-configuration.json]\n- scope: profile\n  description: Access to the end user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/morf-openid-configuration.json]\n- scope: email\n  description: Access to the end user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/morf-openid-configuration.json]\n- scope: phone\n  description: Access to the end user's phone number claim.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/morf-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline API access.\n  flows: [authorizationCode]\n  sources: [well-known/morf-openid-configuration.json]\n- scope: full_access\n  description: >-\n    Full access scope advertised by the OpenID Connect discovery document\n    (scopes_supported). Grants broad access to the Morf API.\n  flows: [authorizationCode]\n  sources: [well-known/morf-openid-configuration.json]\nnotes: >-\n  Scopes harvested verbatim from the live OpenID Connect discovery document\n  scopes_supported list. The API-host RFC 8414 document advertises only the\n  \"email\" scope; the auth-host OIDC document is the fuller set captured here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morf/refs/heads/main/scopes/morf-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Healthcare
- Health IT
- Automation
- Integration
- iPaaS
- Webhooks
- EHR
- Patient Communication
- HIPAA
- Workflow
- Digital Health
token_urls:
- https://auth.morf.health/v1/oauth2/token
---
