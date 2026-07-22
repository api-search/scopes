---
authorization_urls: []
description: ''
docs: https://dp.getweave.com/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Weave Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Weave publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Weave API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Weave
provider_slug: weave
schemes:
- authorizationUrl: https://oidc.weaveconnect.com/oauth2/auth
  name: WeaveOIDC
  source: well-known/weave-openid-configuration.json
  tokenUrl: https://oidc.weaveconnect.com/oauth2/token
  type: openIdConnect
scope_count: 3
scope_names:
- openid
- offline_access
- offline
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the authenticated Weave user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Request a refresh token so the app can obtain new access tokens without re-prompting the user (OIDC offline access).
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy offline-access alias advertised by the Weave authorization server for long-lived refresh-token grants.
  flows:
  - authorizationCode
  scope: offline
slug: weave-scopes
source_filename: weave-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://oidc.weaveconnect.com/.well-known/openid-configuration\ndocs: https://dp.getweave.com/docs\nschemes:\n- name: WeaveOIDC\n  source: well-known/weave-openid-configuration.json\n  type: openIdConnect\n  authorizationUrl: https://oidc.weaveconnect.com/oauth2/auth\n  tokenUrl: https://oidc.weaveconnect.com/oauth2/token\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication; returns an ID token identifying the\n    authenticated Weave user.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/weave-openid-configuration.json\n- scope: offline_access\n  description: >-\n    Request a refresh token so the app can obtain new access tokens without\n    re-prompting the user (OIDC offline access).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/weave-openid-configuration.json\n- scope: offline\n  description: >-\n    Legacy offline-access alias advertised by the Weave\
  \ authorization server for\n    long-lived refresh-token grants.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/weave-openid-configuration.json\nnotes: >-\n  These are the scopes advertised by the Weave OIDC discovery document\n  (scopes_supported). Weave does not publish a granular resource:action\n  permission catalog on its public discovery surface; per-app data permissions\n  are configured in the Weave Developer Portal rather than encoded as OAuth\n  scopes. No spec-derived scopes exist because Weave publishes no public OpenAPI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/scopes/weave-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Communication
- Messaging
- Payments
- Healthcare
- VoIP
- Telephony
- Reviews
- Scheduling
- SMB
- Developer Platform
- OAuth
token_urls: []
---
