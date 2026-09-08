---
api_specs:
- filename: devportal-factiva-products
  format: yaml
  label: Dow Jones Developer Platform
  slug: dow-jones-developer-platform
  spec_type: Postman
  url: https://www.postman.com/dj-cse/workspace/devportal-factiva-products
- filename: dow-jones-developer-platform-newswires-real-time-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Real-Time API
  slug: newswires-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-real-time-api-openapi.yml
- filename: dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Top Stories API
  slug: newswires-top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
- filename: dow-jones-developer-platform-calendar-live-api-openapi.yml
  format: yaml
  label: Dow Jones Calendar Live API
  slug: calendar-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-calendar-live-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-content-api-openapi.yml
  format: yaml
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-content-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
  format: yaml
  label: Factiva Newsletters API
  slug: factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
- filename: dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
  format: yaml
  label: Dow Jones RiskCenter Third Party Platform API
  slug: riskcenter-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Dow Jones Developer Platform Scopes
name_suffix: OAuth Scopes
note: Dow Jones publishes OIDC scopes on its identity service but does NOT publish per-API authorization scopes. The scope string the documented token exchange sends is "openid pib" for every Dow Jones API; entitlement to a given product is carried by the account, not by an OAuth scope. Nothing here is a per-resource permission model.
overview: 'Dow Jones Developer Platform uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dow Jones Developer Platform
provider_slug: dow-jones-developer-platform
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: dow-jones-developer-platform-scopes
source_filename: dow-jones-developer-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://accounts.dowjones.com/.well-known/openid-configuration (200) for scopes_supported; https://developer.dowjones.com/documents/site-docs-newswires_apis-oauth-migration-guide\n  (200) for the scope value the token exchange requires\ndocs: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication\nnote: Dow Jones publishes OIDC scopes on its identity service but does NOT publish per-API authorization\n  scopes. The scope string the documented token exchange sends is \"openid pib\" for every Dow Jones API;\n  entitlement to a given product is carried by the account, not by an OAuth scope. Nothing here is a per-resource\n  permission model.\nissuer: https://sso.accounts.dowjones.com/\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token. Required by the documented jwt-bearer exchange.\n  source: openid-configuration + OAuth Migration Guide\n- name: pib\n  description:\
  \ Dow Jones Professional Information Business audience. Paired with openid in the documented\n    token exchange that yields the bearer token api.dowjones.com accepts.\n  source: OAuth Migration Guide\n- name: profile\n  description: Standard OIDC profile claims.\n  source: openid-configuration scopes_supported\n- name: offline_access\n  description: Issue a refresh token — the credential step 1 of the documented two-step exchange consumes.\n  source: openid-configuration scopes_supported\n- name: email\n  description: Standard OIDC email claim.\n  source: openid-configuration scopes_supported\n- name: email_verified\n  description: Standard OIDC email_verified claim.\n  source: openid-configuration scopes_supported\n- name: given_name\n  description: Standard OIDC given_name claim.\n  source: openid-configuration scopes_supported\n- name: family_name\n  description: Standard OIDC family_name claim.\n  source: openid-configuration scopes_supported\nper_api_scopes:\n  published: false\n\
  \  note: No Dow Jones OpenAPI in openapi/ declares an oauth2 securityScheme, so no per-operation scope\n    requirements exist to derive.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/scopes/dow-jones-developer-platform-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Business Data
- Compliance
- Financial
- Market Data
- News
- Risk and Compliance
- Screening
- Sanctions
token_urls: []
---
