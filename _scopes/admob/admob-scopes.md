---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes#admob
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Admob Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AdMob publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdMob API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdMob
provider_slug: admob
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: GoogleOAuth2
  source: docs
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/admob.readonly
- https://www.googleapis.com/auth/admob.report
scopes:
- description: See your AdMob data. Read-only access to all AdMob data including account information, apps, and ad units.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.readonly
- description: See your AdMob data. Access to generate AdMob ad performance and earnings network and mediation reports.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.report
slug: admob-scopes
source_filename: admob-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.google.com/admob/api/v1/auth\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes#admob\nschemes:\n- name: GoogleOAuth2\n  source: docs\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/admob.readonly\n  description: See your AdMob data. Read-only access to all AdMob data including account information, apps, and ad units.\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: https://www.googleapis.com/auth/admob.report\n  description: See your AdMob data. Access to generate AdMob ad performance and earnings network and mediation reports.\n  flows: [authorizationCode]\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/scopes/admob-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Advertising
- Mobile
- Monetization
- Ads
- Google
- Reporting
- Mediation
- AdTech
token_urls:
- https://oauth2.googleapis.com/token
---
