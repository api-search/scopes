---
authorization_urls:
- https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/authorize
description: ''
docs: https://developer.ehi.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Enterprise Mobility Scopes
name_suffix: OAuth Scopes
note: Enterprise Mobility publishes no scopes reference page. This list is the literal scope set the EHI API Marketplace requests when a developer signs in — extracted from the provider's own published authorize link, not inferred. It scopes the MARKETPLACE's own management surface (browse the catalog, manage client applications, request authorization, manage favorites), not the Rental / Replacement Rental / Commute business APIs, whose scopes are behind the gate and are NOT asserted here. Note the OIDC discovery document advertises only "openid" in scopes_supported — Azure AD B2C does not enumerate resource scopes in discovery, so the authorize link is the authoritative published source.
overview: 'Enterprise Mobility publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Enterprise Mobility API on a user''s behalf.


  Tokens are issued from https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enterprise Mobility
provider_slug: enterprise-mobility
schemes:
- flows:
  - authorizationUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    policy: B2C_1A_SIGNIN
    tokenUrl: https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token
  name: OAuth2AuthorizationCode
  source: authentication/enterprise-mobility-authentication.yml
scope_count: 14
scope_names:
- openid
- offline_access
- https://apimarketplaceprod.onmicrosoft.com/api/api.list
- https://apimarketplaceprod.onmicrosoft.com/api/api.search
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.create
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.read
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.list
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.search
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.manage-owners
- https://apimarketplaceprod.onmicrosoft.com/api/client-application.request-authorization
- https://apimarketplaceprod.onmicrosoft.com/api/member.list
- https://apimarketplaceprod.onmicrosoft.com/api/favorite.create
- https://apimarketplaceprod.onmicrosoft.com/api/favorite.list
- https://apimarketplaceprod.onmicrosoft.com/api/favorite.delete
scopes:
- description: Standard OpenID Connect scope; issues an id_token.
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token so the marketplace session can be renewed.
  flows:
  - authorizationCode
  scope: offline_access
- description: List the APIs in the EHI API Marketplace catalog.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/api.list
- description: Search the EHI API Marketplace catalog.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/api.search
- description: Create a client application registration in the marketplace.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.create
- description: Read a client application registration.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.read
- description: List the caller's client application registrations.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.list
- description: Search client application registrations.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.search
- description: Add or remove owners on a client application registration.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.manage-owners
- description: Request authorization for a client application to consume a specific API. This is the actual access gate — it is a request to Enterprise, not a self-serve grant.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.request-authorization
- description: List the members of the caller's organization in the marketplace.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/member.list
- description: Favorite an API or guide in the marketplace.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.create
- description: List the caller's favorited APIs and guides.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.list
- description: Remove a favorite.
  flows:
  - authorizationCode
  scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.delete
slug: enterprise-mobility-scopes
source_filename: enterprise-mobility-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  The B2C_1A_SIGNIN authorize URL published verbatim in the anonymous page source\n  of https://developer.ehi.com/ and every /apis-overview/ page (scope= query\n  parameter), plus the OIDC discovery documents in well-known/. Probed\n  2026-07-28.\ndocs: https://developer.ehi.com/\nresource: https://apimarketplaceprod.onmicrosoft.com/api\nnote: >-\n  Enterprise Mobility publishes no scopes reference page. This list is the\n  literal scope set the EHI API Marketplace requests when a developer signs in —\n  extracted from the provider's own published authorize link, not inferred. It\n  scopes the MARKETPLACE's own management surface (browse the catalog, manage\n  client applications, request authorization, manage favorites), not the Rental /\n  Replacement Rental / Commute business APIs, whose scopes are behind the gate\n  and are NOT asserted here. Note the OIDC discovery document advertises only\n  \"openid\" in scopes_supported\
  \ — Azure AD B2C does not enumerate resource scopes\n  in discovery, so the authorize link is the authoritative published source.\nschemes:\n  - name: OAuth2AuthorizationCode\n    source: authentication/enterprise-mobility-authentication.yml\n    flows:\n      - flow: authorizationCode\n        policy: B2C_1A_SIGNIN\n        authorizationUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/authorize\n        tokenUrl: >-\n          https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; issues an id_token.\n    flows: [authorizationCode]\n    group: identity\n  - scope: offline_access\n    description: Requests a refresh token so the marketplace session can be renewed.\n    flows: [authorizationCode]\n    group: identity\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/api.list\n    short:\
  \ api.list\n    description: List the APIs in the EHI API Marketplace catalog.\n    flows: [authorizationCode]\n    group: catalog\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/api.search\n    short: api.search\n    description: Search the EHI API Marketplace catalog.\n    flows: [authorizationCode]\n    group: catalog\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.create\n    short: client-application.create\n    description: Create a client application registration in the marketplace.\n    flows: [authorizationCode]\n    group: client-applications\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.read\n    short: client-application.read\n    description: Read a client application registration.\n    flows: [authorizationCode]\n    group: client-applications\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.list\n    short: client-application.list\n    description: List the caller's client\
  \ application registrations.\n    flows: [authorizationCode]\n    group: client-applications\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.search\n    short: client-application.search\n    description: Search client application registrations.\n    flows: [authorizationCode]\n    group: client-applications\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.manage-owners\n    short: client-application.manage-owners\n    description: Add or remove owners on a client application registration.\n    flows: [authorizationCode]\n    group: client-applications\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/client-application.request-authorization\n    short: client-application.request-authorization\n    description: >-\n      Request authorization for a client application to consume a specific API.\n      This is the actual access gate — it is a request to Enterprise, not a\n      self-serve grant.\n    flows: [authorizationCode]\n\
  \    group: client-applications\n    gate: true\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/member.list\n    short: member.list\n    description: List the members of the caller's organization in the marketplace.\n    flows: [authorizationCode]\n    group: organization\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.create\n    short: favorite.create\n    description: Favorite an API or guide in the marketplace.\n    flows: [authorizationCode]\n    group: personalization\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.list\n    short: favorite.list\n    description: List the caller's favorited APIs and guides.\n    flows: [authorizationCode]\n    group: personalization\n  - scope: https://apimarketplaceprod.onmicrosoft.com/api/favorite.delete\n    short: favorite.delete\n    description: Remove a favorite.\n    flows: [authorizationCode]\n    group: personalization\nsummary:\n  total: 14\n  identity: 2\n  resource_scopes: 12\n  groups:\n\
  \    - identity\n    - catalog\n    - client-applications\n    - organization\n    - personalization\nnot_published:\n  - Scopes for the Rental, Replacement Rental and Commute business-line APIs\n  - Any scope-to-permission or scope-to-role mapping document\n  - Consent screen copy or admin-consent requirements\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enterprise-mobility/refs/heads/main/scopes/enterprise-mobility-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Travel
- United States
- Car Rental
- Ground Transportation
- Mobility
- Corporate Travel
- Distribution
- Fleet Management
- Insurance Replacement Rental
- Booking
token_urls:
- https://apimarketplaceprod.b2clogin.com/apimarketplaceprod.onmicrosoft.com/b2c_1a_signin/oauth2/v2.0/token
---
