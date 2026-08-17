---
api_specs:
- filename: google-indexing-urlnotifications-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications API
  slug: google-indexing-urlnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-api-openapi.yml
- filename: google-indexing-urlnotifications-publish-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications:publish API
  slug: google-indexing-urlnotifications-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-publish-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/search/apis/indexing-api/v3/prereqs
flows:
- jwt-bearer
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Indexing Scopes
name_suffix: OAuth Scopes
note: 'Upgraded from derived to searched on 2026-08-13. The scope string and its description were read from Google''s live Discovery Document (revision 20260805), which is the authoritative publisher of this API''s auth.oauth2.scopes block — Google''s own description is "Submit data to Google for indexing", which the derived baseline had paraphrased. There is exactly ONE scope, it is coarse, and it covers both operations: there is no read-only scope for getMetadata.'
overview: 'Google Indexing publishes 1 OAuth 2.0 scope via the jwt-bearer and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Indexing API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Indexing
provider_slug: google-indexing
schemes:
- flows:
  - flow: jwt-bearer
    tokenUrl: https://oauth2.googleapis.com/token
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/_original/google-indexing-discovery-v3.json
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/indexing
scopes:
- description: Submit data to Google for indexing
  flows:
  - jwt-bearer
  - authorizationCode
  scope: https://www.googleapis.com/auth/indexing
slug: google-indexing-scopes
source_filename: google-indexing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://indexing.googleapis.com/$discovery/rest?version=v3\ndocs: https://developers.google.com/search/apis/indexing-api/v3/prereqs\nnote: >-\n  Upgraded from derived to searched on 2026-08-13. The scope string and its description were read from\n  Google's live Discovery Document (revision 20260805), which is the authoritative publisher of this\n  API's auth.oauth2.scopes block — Google's own description is \"Submit data to Google for indexing\",\n  which the derived baseline had paraphrased. There is exactly ONE scope, it is coarse, and it covers\n  both operations: there is no read-only scope for getMetadata.\nschemes:\n  - name: OAuth2\n    source: openapi/_original/google-indexing-discovery-v3.json\n    flows:\n      - flow: jwt-bearer\n        tokenUrl: https://oauth2.googleapis.com/token\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n\
  scopes:\n  - scope: https://www.googleapis.com/auth/indexing\n    description: Submit data to Google for indexing\n    sensitivity: restricted\n    grants:\n      - publishUrlNotification\n      - getUrlNotificationMetadata\n    flows:\n      - jwt-bearer\n      - authorizationCode\n    sources:\n      - openapi/_original/google-indexing-discovery-v3.json\n      - openapi/google-indexing-urlnotifications-publish-api-openapi.yml\n      - openapi/google-indexing-urlnotifications-api-openapi.yml\ngranularity:\n  scope_count: 1\n  read_only_scope: false\n  least_privilege_possible: false\n  note: >-\n    A single scope covers both the read operation and the production write. An agent that only needs to\n    look up notification metadata must be granted the same scope that lets it change what Google\n    crawls. This is a real least-privilege gap in the provider's design, not a gap in this artifact.\nauthorization_beyond_scope:\n  required: true\n  mechanism: Search Console delegated site ownership,\
  \ enforced per URL\n  artifact: authentication/google-indexing-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/scopes/google-indexing-scopes.yml
summary_line: 1 scope · jwt-bearer/authorizationCode
tags:
- Crawling
- Google
- Indexing
- Search
- SEO
- URLs
token_urls:
- https://oauth2.googleapis.com/token
---
