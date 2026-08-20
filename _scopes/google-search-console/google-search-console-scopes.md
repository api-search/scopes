---
api_specs:
- filename: google-search-console-url-testing-tools-api-openapi.yml
  format: yaml
  label: Google Search Console URL Testing Tools API
  slug: google-search-console-url-testing-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-url-testing-tools-api-openapi.yml
- filename: google-search-console-indexing-api-openapi.yml
  format: yaml
  label: Google Indexing API
  slug: google-indexing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-indexing-api-openapi.yml
- filename: google-search-console-search-analytics-api-openapi.yml
  format: yaml
  label: Google Search Console Search Analytics API
  slug: google-search-console-search-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-search-analytics-api-openapi.yml
- filename: google-search-console-sitemaps-api-openapi.yml
  format: yaml
  label: Google Search Console Sitemaps API
  slug: google-search-console-sitemaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sitemaps-api-openapi.yml
- filename: google-search-console-sites-api-openapi.yml
  format: yaml
  label: Google Search Console Sites API
  slug: google-search-console-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sites-api-openapi.yml
- filename: google-search-console-url-inspection-api-openapi.yml
  format: yaml
  label: Google Search Console URL Inspection API
  slug: google-search-console-url-inspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-url-inspection-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes#searchconsole
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Search Console Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Search Console publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Search Console API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Search Console
provider_slug: google-search-console
schemes:
- description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-indexing-api-openapi.yml
- description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the webmasters or webmasters.readonly scope depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-search-analytics-api-openapi.yml
- description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the webmasters or webmasters.readonly scope depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-sitemaps-api-openapi.yml
- description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the webmasters or webmasters.readonly scope depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-sites-api-openapi.yml
- description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the webmasters or webmasters.readonly scope depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-url-inspection-api-openapi.yml
- description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-url-testing-tools-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/indexing
- https://www.googleapis.com/auth/webmasters
- https://www.googleapis.com/auth/webmasters.readonly
scopes:
- description: Submit data to Google for indexing
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/indexing
- description: View and manage Search Console data for your verified sites
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/webmasters
- description: View Search Console data for your verified sites
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/webmasters.readonly
slug: google-search-console-scopes
source_filename: google-search-console-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes#searchconsole\nsource: >-\n  Scope strings and descriptions confirmed verbatim against Google's own Discovery documents\n  (auth.oauth2.scopes) fetched live on 2026-08-13 from\n  https://searchconsole.googleapis.com/$discovery/rest?version=v1 and\n  https://indexing.googleapis.com/$discovery/rest?version=v3, and against the OAuth 2.0 Scopes for\n  Google APIs reference. Baseline derived from openapi/google-search-console-indexing-api-openapi.yml, openapi/google-search-console-search-analytics-api-openapi.yml,\n  openapi/google-search-console-sitemaps-api-openapi.yml, openapi/google-search-console-sites-api-openapi.yml,\n  openapi/google-search-console-url-inspection-api-openapi.yml, openapi/google-search-console-url-testing-tools-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-search-console-indexing-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'\n- name: OAuth2\n  source: openapi/google-search-console-search-analytics-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the\n    webmasters or webmasters.readonly scope depending on the operation.\n- name: OAuth2\n  source: openapi/google-search-console-sitemaps-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the\n\
  \    webmasters or webmasters.readonly scope depending on the operation.\n- name: OAuth2\n  source: openapi/google-search-console-sites-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the\n    webmasters or webmasters.readonly scope depending on the operation.\n- name: OAuth2\n  source: openapi/google-search-console-url-inspection-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the\n    webmasters or webmasters.readonly scope depending on the operation.\n- name: OAuth2\n  source: openapi/google-search-console-url-testing-tools-api-openapi.yml\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: 'Google OAuth 2.0. Authorization server metadata: https://accounts.google.com/.well-known/openid-configuration'\nscopes:\n- scope: https://www.googleapis.com/auth/indexing\n  description: Submit data to Google for indexing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-search-console-indexing-api-openapi.yml\n- scope: https://www.googleapis.com/auth/webmasters\n  description: View and manage Search Console data for your verified sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-search-console-search-analytics-api-openapi.yml\n  - openapi/google-search-console-sitemaps-api-openapi.yml\n  - openapi/google-search-console-sites-api-openapi.yml\n  - openapi/google-search-console-url-inspection-api-openapi.yml\n  - openapi/google-search-console-url-testing-tools-api-openapi.yml\n- scope: https://www.googleapis.com/auth/webmasters.readonly\n\
  \  description: View Search Console data for your verified sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-search-console-search-analytics-api-openapi.yml\n  - openapi/google-search-console-sitemaps-api-openapi.yml\n  - openapi/google-search-console-sites-api-openapi.yml\n  - openapi/google-search-console-url-inspection-api-openapi.yml\n  - openapi/google-search-console-url-testing-tools-api-openapi.yml\nnotes:\n- >-\n  Three scopes across two hosts. webmasters and webmasters.readonly cover searchconsole.googleapis.com;\n  indexing is a separate scope for indexing.googleapis.com and is not interchangeable with them.\n- >-\n  urlTestingTools.mobileFriendlyTest.run declares NO scope in the Discovery document — the only\n  operation on this surface that does not require one.\n- >-\n  Scope alone is not access. Search Console authorizes per verified property: the token must belong\n  to an account that owns or is delegated on the property, and for the Indexing API the\
  \ service\n  account must be added as an Owner inside Search Console.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/scopes/google-search-console-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Analytics
- Google
- Indexing
- Search
- Search Analytics
- SEO
- Sitemap
- URL Inspection
- Webmaster Tools
token_urls:
- https://oauth2.googleapis.com/token
---
