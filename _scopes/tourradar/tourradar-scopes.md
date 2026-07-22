---
authorization_urls:
- https://auth.tourradar.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tourradar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TourRadar publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TourRadar API on a user''s behalf.


  Tokens are issued from https://auth.tourradar.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TourRadar
provider_slug: tourradar
schemes:
- flows:
  - authorizationUrl: https://auth.tourradar.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tourradar.com/oauth2/token
  name: TourRadarB2BOAuth
  source: https://dashboard.api.b2b.tourradar.com/config.js
scope_count: 24
scope_names:
- com.tourradar.bookings.affiliate/read
- com.tourradar.bookings/read
- com.tourradar.bookings/selfRead
- com.tourradar.credentials/read
- com.tourradar.credentials/write
- com.tourradar.operators/read
- com.tourradar.partners.apps/read
- com.tourradar.partners.apps/write
- com.tourradar.partners.customizations/read
- com.tourradar.partners.customizations/write
- com.tourradar.partners.domains/read
- com.tourradar.partners.domains/write
- com.tourradar.partners.openapi/read
- com.tourradar.partners.payments.methods/read
- com.tourradar.partners.payments.methods/write
- com.tourradar.partners.users/read
- com.tourradar.partners.users/selfWrite
- com.tourradar.partners.users/write
- com.tourradar.partners/admin
- com.tourradar.partners/read
- com.tourradar.partners/write
- openid
- email
- profile
scopes:
- description: Read affiliate bookings.
  flows: []
  scope: com.tourradar.bookings.affiliate/read
- description: Read bookings.
  flows: []
  scope: com.tourradar.bookings/read
- description: Read the caller's own bookings.
  flows: []
  scope: com.tourradar.bookings/selfRead
- description: Read API credentials.
  flows: []
  scope: com.tourradar.credentials/read
- description: Manage API credentials.
  flows: []
  scope: com.tourradar.credentials/write
- description: Read tour operator data.
  flows: []
  scope: com.tourradar.operators/read
- description: Read partner applications.
  flows: []
  scope: com.tourradar.partners.apps/read
- description: Manage partner applications.
  flows: []
  scope: com.tourradar.partners.apps/write
- description: Read partner customizations.
  flows: []
  scope: com.tourradar.partners.customizations/read
- description: Manage partner customizations.
  flows: []
  scope: com.tourradar.partners.customizations/write
- description: Read partner domains.
  flows: []
  scope: com.tourradar.partners.domains/read
- description: Manage partner domains.
  flows: []
  scope: com.tourradar.partners.domains/write
- description: Read the partner-facing OpenAPI definition.
  flows: []
  scope: com.tourradar.partners.openapi/read
- description: Read partner payment methods.
  flows: []
  scope: com.tourradar.partners.payments.methods/read
- description: Manage partner payment methods.
  flows: []
  scope: com.tourradar.partners.payments.methods/write
- description: Read partner users.
  flows: []
  scope: com.tourradar.partners.users/read
- description: Update the caller's own partner user profile.
  flows: []
  scope: com.tourradar.partners.users/selfWrite
- description: Manage partner users.
  flows: []
  scope: com.tourradar.partners.users/write
- description: Administer the partner account.
  flows: []
  scope: com.tourradar.partners/admin
- description: Read partner account data.
  flows: []
  scope: com.tourradar.partners/read
- description: Manage partner account data.
  flows: []
  scope: com.tourradar.partners/write
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: OIDC email claim.
  flows: []
  scope: email
- description: OIDC profile claims.
  flows: []
  scope: profile
slug: tourradar-scopes
source_filename: tourradar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://dashboard.api.b2b.tourradar.com/config.js\nnotes: >-\n  OAuth scope list published in the public config.js of the TourRadar partner\n  dashboard (dashboard.api.b2b.tourradar.com). Scopes follow an AWS Cognito\n  resource-server convention (com.tourradar.<resource>/<action>). Descriptions\n  below are mechanical readings of the scope identifier, not provider-authored\n  text. Notably, the com.tourradar.partners.openapi/read scope indicates an\n  OpenAPI definition is served to authenticated partners.\nschemes:\n  - name: TourRadarB2BOAuth\n    source: https://dashboard.api.b2b.tourradar.com/config.js\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.tourradar.com/oauth2/authorize\n        tokenUrl: https://auth.tourradar.com/oauth2/token\nscopes:\n  - scope: com.tourradar.bookings.affiliate/read\n    description: Read affiliate bookings.\n  - scope: com.tourradar.bookings/read\n   \
  \ description: Read bookings.\n  - scope: com.tourradar.bookings/selfRead\n    description: Read the caller's own bookings.\n  - scope: com.tourradar.credentials/read\n    description: Read API credentials.\n  - scope: com.tourradar.credentials/write\n    description: Manage API credentials.\n  - scope: com.tourradar.operators/read\n    description: Read tour operator data.\n  - scope: com.tourradar.partners.apps/read\n    description: Read partner applications.\n  - scope: com.tourradar.partners.apps/write\n    description: Manage partner applications.\n  - scope: com.tourradar.partners.customizations/read\n    description: Read partner customizations.\n  - scope: com.tourradar.partners.customizations/write\n    description: Manage partner customizations.\n  - scope: com.tourradar.partners.domains/read\n    description: Read partner domains.\n  - scope: com.tourradar.partners.domains/write\n    description: Manage partner domains.\n  - scope: com.tourradar.partners.openapi/read\n    description:\
  \ Read the partner-facing OpenAPI definition.\n  - scope: com.tourradar.partners.payments.methods/read\n    description: Read partner payment methods.\n  - scope: com.tourradar.partners.payments.methods/write\n    description: Manage partner payment methods.\n  - scope: com.tourradar.partners.users/read\n    description: Read partner users.\n  - scope: com.tourradar.partners.users/selfWrite\n    description: Update the caller's own partner user profile.\n  - scope: com.tourradar.partners.users/write\n    description: Manage partner users.\n  - scope: com.tourradar.partners/admin\n    description: Administer the partner account.\n  - scope: com.tourradar.partners/read\n    description: Read partner account data.\n  - scope: com.tourradar.partners/write\n    description: Manage partner account data.\n  - scope: openid\n    description: OpenID Connect authentication.\n  - scope: email\n    description: OIDC email claim.\n  - scope: profile\n    description: OIDC profile claims.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/scopes/tourradar-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Travel
- Tours
- Booking
- Marketplace
- Adventure Travel
- Distribution
- Affiliates
token_urls:
- https://auth.tourradar.com/oauth2/token
---
