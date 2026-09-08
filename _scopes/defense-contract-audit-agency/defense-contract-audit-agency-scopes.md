---
authorization_urls:
- https://piee.eb.mil/portal/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Defense Contract Audit Agency Scopes
name_suffix: OAuth Scopes
note: DCAA publishes no scope or permission reference. The only OAuth scopes observable anywhere on a DCAA host are the two standard OpenID Connect scopes the Contractor Submission Portal requests from DoD PIEE. The public Branch Locator API has no OAuth surface at all. This is a two-scope sign-in, not a developer authorization model.
overview: 'Defense Contract Audit Agency publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Defense Contract Audit Agency API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Defense Contract Audit Agency
provider_slug: defense-contract-audit-agency
schemes:
- flows:
  - authorizationUrl: https://piee.eb.mil/portal/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: null
  name: piee-oidc
  source: probed https://csp.dcaa.mil/ (302 to PIEE authorize endpoint)
scope_count: 2
scope_names:
- openid
- profile
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the signed-in DoD PIEE user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect scope requesting the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: defense-contract-audit-agency-scopes
source_filename: defense-contract-audit-agency-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://csp.dcaa.mil/ sign-in redirect observed 2026-09-07 — the scope set is read from\n  the live authorization request DCAA's own client builds, not from any published document.\nnote: >-\n  DCAA publishes no scope or permission reference. The only OAuth scopes observable\n  anywhere on a DCAA host are the two standard OpenID Connect scopes the Contractor\n  Submission Portal requests from DoD PIEE. The public Branch Locator API has no OAuth\n  surface at all. This is a two-scope sign-in, not a developer authorization model.\ndocs: null\nschemes:\n  - name: piee-oidc\n    source: probed https://csp.dcaa.mil/ (302 to PIEE authorize endpoint)\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://piee.eb.mil/portal/oauth2/authorize\n        tokenUrl: null\n        pkce: S256\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope requesting an ID token for the signed-in DoD\
  \ PIEE user.\n    flows: [authorizationCode]\n    sources: [probed https://csp.dcaa.mil/]\n  - scope: profile\n    description: Standard OpenID Connect scope requesting the user's basic profile claims.\n    flows: [authorizationCode]\n    sources: [probed https://csp.dcaa.mil/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-contract-audit-agency/refs/heads/main/scopes/defense-contract-audit-agency-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Federal-Government
- Defense
- Department of Defense
- Audit
- Contract Audit
- Financial
- Government Contracting
- CAGE Code
- Unique Entity Identifier
- Locator
token_urls: []
---
