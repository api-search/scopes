---
api_specs:
- filename: iso-15143-3-aemp-20-api-postman-collection
  format: yaml
  label: ISO 15143-3 (AEMP 2.0) API
  slug: iso-15143-3-aemp-api
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/iso-15143-3-aemp-20-api-postman-collection
- filename: visionlink-apis-postman-collection
  format: yaml
  label: VisionLink APIs
  slug: visionlink-apis
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/visionlink-apis-postman-collection
authorization_urls:
- https://fedlogin.cat.com/as/authorization.oauth2
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Caterpillar Scopes
name_suffix: OAuth Scopes
note: Read from `scopes_supported` in the live OIDC discovery document served by Caterpillar's PingFederate authorization server (HTTP 200, 2026-09-05). This is the authorization server's full advertised scope set across every client it serves — Caterpillar publishes no per-API scope reference page, and the Cat Digital developer guides describe the client-credentials exchange without naming scopes, so which of these an ISO 15143-3 or VisionLink subscription is actually granted is not publicly stated. Descriptions below are the standard OIDC meanings where they apply; the Caterpillar-specific scopes carry no published description and are recorded without one rather than guessed at.
overview: 'Caterpillar publishes 13 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Caterpillar API on a user''s behalf.


  Tokens are issued from https://fedlogin.cat.com/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Caterpillar
provider_slug: caterpillar
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://fedlogin.cat.com/as/token.oauth2
  - authorizationUrl: https://fedlogin.cat.com/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://fedlogin.cat.com/as/token.oauth2
  name: CatDigitalOAuth2
  source: https://fedlogin.cat.com/.well-known/openid-configuration
scope_count: 13
scope_names:
- openid
- profile
- email
- address
- phone_number
- read:all
- write:all
- manage:all
- import:all
- affiliate:all
- session:role-any
- user_impersonation
- WINDCHILL_READ
scopes:
- description: OpenID Connect — request an ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (displayName, givenName, sn).
  flows: []
  scope: profile
- description: Standard OIDC email claim (mail).
  flows: []
  scope: email
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Phone claim (telephonenumber).
  flows: []
  scope: phone_number
- description: ''
  flows: []
  scope: read:all
- description: ''
  flows: []
  scope: write:all
- description: ''
  flows: []
  scope: manage:all
- description: ''
  flows: []
  scope: import:all
- description: ''
  flows: []
  scope: affiliate:all
- description: ''
  flows: []
  scope: session:role-any
- description: ''
  flows: []
  scope: user_impersonation
- description: ''
  flows: []
  scope: WINDCHILL_READ
slug: caterpillar-scopes
source_filename: caterpillar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://fedlogin.cat.com/.well-known/openid-configuration\nnote: >-\n  Read from `scopes_supported` in the live OIDC discovery document served by\n  Caterpillar's PingFederate authorization server (HTTP 200, 2026-09-05). This is\n  the authorization server's full advertised scope set across every client it\n  serves — Caterpillar publishes no per-API scope reference page, and the Cat\n  Digital developer guides describe the client-credentials exchange without naming\n  scopes, so which of these an ISO 15143-3 or VisionLink subscription is actually\n  granted is not publicly stated. Descriptions below are the standard OIDC\n  meanings where they apply; the Caterpillar-specific scopes carry no published\n  description and are recorded without one rather than guessed at.\ndocs: null\nschemes:\n  - name: CatDigitalOAuth2\n    source: https://fedlogin.cat.com/.well-known/openid-configuration\n    flows:\n      - flow: clientCredentials\n\
  \        tokenUrl: https://fedlogin.cat.com/as/token.oauth2\n      - flow: authorizationCode\n        authorizationUrl: https://fedlogin.cat.com/as/authorization.oauth2\n        tokenUrl: https://fedlogin.cat.com/as/token.oauth2\nscopes:\n  - scope: openid\n    description: OpenID Connect — request an ID token.\n    standard: true\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: profile\n    description: Standard OIDC profile claims (displayName, givenName, sn).\n    standard: true\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: email\n    description: Standard OIDC email claim (mail).\n    standard: true\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: address\n    description: Standard OIDC address claim.\n    standard: true\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: phone_number\n    description: Phone claim (telephonenumber).\n \
  \   standard: false\n    note: Non-standard spelling of the OIDC `phone` scope.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: read:all\n    description: null\n    note: Caterpillar-specific; no published description.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: write:all\n    description: null\n    note: Caterpillar-specific; no published description.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: manage:all\n    description: null\n    note: Caterpillar-specific; no published description.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: import:all\n    description: null\n    note: Caterpillar-specific; no published description.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: affiliate:all\n    description: null\n    note: Caterpillar-specific; likely tied to the catafltncode / catafltnclass claims.\n\
  \    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: session:role-any\n    description: null\n    note: Caterpillar-specific session/role scope.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: user_impersonation\n    description: null\n    note: Caterpillar-specific; delegated/impersonated access.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\n  - scope: WINDCHILL_READ\n    description: null\n    note: >-\n      Caterpillar-specific; names PTC Windchill (PLM), i.e. this authorization\n      server fronts internal enterprise systems as well as the public API estate.\n    sources: [https://fedlogin.cat.com/.well-known/openid-configuration]\ncoverage:\n  scopes_advertised: 13\n  scopes_with_published_description: 4\n  per_api_scope_reference_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caterpillar/refs/heads/main/scopes/caterpillar-scopes.yml
summary_line: 13 scopes · clientCredentials/authorizationCode
tags:
- Construction
- Engines
- Fortune 500
- Heavy Equipment
- Locomotives
- Manufacturing
- Mining
- Telematics
- Fleet Management
- ISO 15143-3
- AEMP
token_urls:
- https://fedlogin.cat.com/as/token.oauth2
---
