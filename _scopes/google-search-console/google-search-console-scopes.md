---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Search Console Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Search Console publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Search Console API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Search Console
provider_slug: google-search-console
schemes:
- description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the webmasters or webmasters.readonly scope depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-search-console-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/webmasters
- https://www.googleapis.com/auth/webmasters.readonly
scopes:
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
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-search-console-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-search-console-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Google Search Console data. Requires the\n    webmasters or webmasters.readonly scope depending on the operation.\nscopes:\n- scope: https://www.googleapis.com/auth/webmasters\n  description: View and manage Search Console data for your verified sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-search-console-api-openapi.yml\n- scope: https://www.googleapis.com/auth/webmasters.readonly\n  description: View Search Console data for your verified sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-search-console-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/scopes/google-search-console-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
token_urls:
- https://oauth2.googleapis.com/token
---
