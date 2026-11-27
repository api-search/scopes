---
api_specs:
- filename: google-safe-browsing-hashes-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hashes API
  slug: google-safe-browsing-hashes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashes-api-openapi.yml
- filename: google-safe-browsing-hashlist-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hash List API
  slug: google-safe-browsing-hashlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashlist-api-openapi.yml
- filename: google-safe-browsing-hashlists-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hash Lists API
  slug: google-safe-browsing-hashlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashlists-api-openapi.yml
- filename: google-safe-browsing-projects-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Projects API
  slug: google-safe-browsing-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-projects-api-openapi.yml
- filename: google-safe-browsing-threatlists-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Threat Lists API
  slug: google-safe-browsing-threatlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-threatlists-api-openapi.yml
- filename: google-safe-browsing-uris-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Uris API
  slug: google-safe-browsing-uris-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-uris-api-openapi.yml
- filename: google-safe-browsing-urls-api-openapi.yml
  format: yaml
  label: Google Safe Browsing URLs API
  slug: google-safe-browsing-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-urls-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Safe Browsing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Safe Browsing publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Safe Browsing API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Safe Browsing
provider_slug: google-safe-browsing
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-safe-browsing-webrisk-hashes-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-safe-browsing-webrisk-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-safe-browsing-webrisk-threat-lists-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-safe-browsing-webrisk-uris-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-safe-browsing-scopes
source_filename: google-safe-browsing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-safe-browsing-webrisk-hashes-api-openapi.yml, openapi/google-safe-browsing-webrisk-projects-api-openapi.yml,\n  openapi/google-safe-browsing-webrisk-threat-lists-api-openapi.yml, openapi/google-safe-browsing-webrisk-uris-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-safe-browsing-webrisk-hashes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-safe-browsing-webrisk-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-safe-browsing-webrisk-threat-lists-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-safe-browsing-webrisk-uris-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-safe-browsing-webrisk-hashes-api-openapi.yml\n  - openapi/google-safe-browsing-webrisk-projects-api-openapi.yml\n  - openapi/google-safe-browsing-webrisk-threat-lists-api-openapi.yml\n  - openapi/google-safe-browsing-webrisk-uris-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-safe-browsing/scopes/google-safe-browsing-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Google
- Malware
- Safe Browsing
- Security
- Threats
- URLs
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
