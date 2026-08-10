---
authorization_urls:
- https://login.accessfintech.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Accessfintech Scopes
name_suffix: OAuth Scopes
note: IMPORTANT SCOPE OF THIS FILE. AccessFintech publishes no OpenAPI and no public scopes / permissions reference, so nothing here is a business scope for the Synergy API. These are the scopes the company's own OpenID Connect issuer advertises in its anonymous discovery document. The `openid`-family scopes are the standard OIDC set the Synergy sign-in flow can request; the `okta.*` scopes belong to the Okta org management authorization server that the same issuer fronts, not to the Synergy data API. Recorded as observed, not as a claim about AccessFintech's API authorization model.
overview: 'AccessFintech publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AccessFintech API on a user''s behalf.


  Tokens are issued from https://login.accessfintech.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AccessFintech
provider_slug: accessfintech
schemes:
- flows:
  - authorizationUrl: https://login.accessfintech.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.accessfintech.com/oauth2/v1/token
  - authorizationUrl: https://login.accessfintech.com/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://login.accessfintech.com/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://login.accessfintech.com/oauth2/v1/token
  issuer: https://login.accessfintech.com
  name: openid-connect
  source: https://login.accessfintech.com/.well-known/openid-configuration
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: Request an ID token; required to initiate an OpenID Connect flow.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows: []
  scope: profile
- description: The email and email_verified claims.
  flows: []
  scope: email
- description: The address claim.
  flows: []
  scope: address
- description: The phone_number claim.
  flows: []
  scope: phone
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows: []
  scope: offline_access
- description: Group memberships for the authenticated user — the entitlement carrier for tenant/org access in the Synergy UI.
  flows: []
  scope: groups
slug: accessfintech-scopes
source_filename: accessfintech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://login.accessfintech.com/.well-known/openid-configuration\nnote: >-\n  IMPORTANT SCOPE OF THIS FILE. AccessFintech publishes no OpenAPI and no public scopes /\n  permissions reference, so nothing here is a business scope for the Synergy API. These are\n  the scopes the company's own OpenID Connect issuer advertises in its anonymous discovery\n  document. The `openid`-family scopes are the standard OIDC set the Synergy sign-in flow\n  can request; the `okta.*` scopes belong to the Okta org management authorization server\n  that the same issuer fronts, not to the Synergy data API. Recorded as observed, not as a\n  claim about AccessFintech's API authorization model.\n\nschemes:\n  - name: openid-connect\n    issuer: https://login.accessfintech.com\n    source: https://login.accessfintech.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.accessfintech.com/oauth2/v1/authorize\n\
  \        tokenUrl: https://login.accessfintech.com/oauth2/v1/token\n      - flow: implicit\n        authorizationUrl: https://login.accessfintech.com/oauth2/v1/authorize\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://login.accessfintech.com/oauth2/v1/device/authorize\n        tokenUrl: https://login.accessfintech.com/oauth2/v1/token\n\nscopes:\n  - scope: openid\n    description: Request an ID token; required to initiate an OpenID Connect flow.\n    kind: oidc-standard\n    flows: [authorizationCode, implicit, deviceCode]\n  - scope: profile\n    description: Basic profile claims (name, preferred_username, locale, updated_at).\n    kind: oidc-standard\n  - scope: email\n    description: The email and email_verified claims.\n    kind: oidc-standard\n  - scope: address\n    description: The address claim.\n    kind: oidc-standard\n  - scope: phone\n    description: The phone_number claim.\n    kind: oidc-standard\n  - scope: offline_access\n    description: Issue a refresh\
  \ token so the client can renew access without re-prompting.\n    kind: oidc-standard\n  - scope: groups\n    description: Group memberships for the authenticated user — the entitlement carrier for tenant/org access in the Synergy UI.\n    kind: okta\n\norg_management_scopes:\n  note: >-\n    The RFC 8414 metadata document additionally advertises the full Okta org management\n    scope family (okta.users.*, okta.groups.*, okta.apps.*, okta.policies.*, okta.logs.read,\n    okta.sessions.*, and ~40 more read/manage pairs). These are Okta platform administration\n    scopes exposed by every Okta org, not AccessFintech product scopes, and they are listed\n    here only so the observation is not silently dropped. See\n    well-known/accessfintech-oauth-authorization-server.json for the verbatim list.\n  count: 82\n  source: well-known/accessfintech-oauth-authorization-server.json\n\nsynergy_api_scopes: unknown\nsynergy_api_scopes_note: >-\n  The Synergy GraphQL/REST surface at https://api.accessfintech.com\
  \ is behind a CloudFront\n  WAF and an authenticated session; no scope or permission reference is published publicly.\n\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n    - url: https://login.accessfintech.com/.well-known/openid-configuration\n      status: 200\n    - url: https://login.accessfintech.com/.well-known/oauth-authorization-server\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessfintech/refs/heads/main/scopes/accessfintech-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/deviceCode
tags:
- Company
- Financial Services
- Capital Markets
- Post-Trade
- Settlement
- Data Networks
- Reconciliation
- Fintech
- GraphQL
token_urls:
- https://login.accessfintech.com/oauth2/v1/token
---
