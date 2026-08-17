---
api_specs:
- filename: google-admob-api-v1-openapi.yml
  format: yaml
  label: Google AdMob API v1
  slug: google-admob-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-api-v1-openapi.yml
- filename: google-admob-api-v1beta-openapi.yml
  format: yaml
  label: Google AdMob API v1beta
  slug: google-admob-api-v1beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/openapi/google-admob-api-v1beta-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/admob/api/v1/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Admob Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google AdMob publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google AdMob API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google AdMob
provider_slug: google-admob
schemes:
- description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: GoogleOAuth2
  source: openapi/google-admob-api-v1-openapi.yml
- description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: GoogleOAuth2
  source: openapi/google-admob-api-v1beta-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/admob.readonly
- https://www.googleapis.com/auth/admob.report
scopes:
- description: See your AdMob data. Grants read access to account, app, ad unit, ad source, adapter, ad unit mapping and mediation group resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.readonly
- description: See your AdMob data. Grants access to generate network, mediation and campaign reports.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/admob.report
slug: google-admob-scopes
source_filename: google-admob-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/google-admob-api-v1-openapi.yml, openapi/google-admob-api-v1beta-openapi.yml\nschemes:\n- name: GoogleOAuth2\n  source: openapi/google-admob-api-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.\n- name: GoogleOAuth2\n  source: openapi/google-admob-api-v1beta-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 user authorization. AdMob does not support service accounts.\nscopes:\n- scope: https://www.googleapis.com/auth/admob.readonly\n  description: See your AdMob data. Grants read access to account, app, ad unit, ad source, adapter, ad\n    unit mapping\
  \ and mediation group resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-admob-api-v1-openapi.yml\n  - openapi/google-admob-api-v1beta-openapi.yml\n- scope: https://www.googleapis.com/auth/admob.report\n  description: See your AdMob data. Grants access to generate network, mediation and campaign reports.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-admob-api-v1-openapi.yml\n  - openapi/google-admob-api-v1beta-openapi.yml\ndocs: https://developers.google.com/admob/api/v1/getting-started\nnotes: 'Scopes confirmed against Google''s own AdMob Discovery Document auth block (both v1 and v1beta\n  declare exactly these two) and the AdMob getting-started page on 2026-08-13. AdMob publishes only two\n  scopes and neither is a write scope: there is no admob.write. The v1beta write methods are authorized\n  by the same admob.readonly/admob.report tokens plus the consenting user''s AdMob account role, which\n  means SCOPE ALONE CANNOT CONSTRAIN AN AGENT\
  \ TO READ-ONLY on v1beta. To keep an agent read-only, restrict\n  it to the v1 channel, which has no write operations at all.'\nwrite_scope_published: false\nagent_note: Neither scope is write-scoped; v1beta writes ride on the same tokens. Channel choice, not\n  scope choice, is the read-only control.\ncross_links:\n  authentication: authentication/google-admob-authentication.yml\n  wellknown: well-known/google-admob-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-admob/refs/heads/main/scopes/google-admob-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Ad Mediation
- AdMob
- Advertising
- App Monetization
- Mobile Advertising
- Mobile Apps
- Reports
- Reporting
token_urls:
- https://oauth2.googleapis.com/token
---
