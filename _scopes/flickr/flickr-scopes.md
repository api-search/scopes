---
authorization_urls:
- https://www.flickr.com/services/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Flickr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flickr publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flickr API on a user''s behalf.


  Tokens are issued from https://www.flickr.com/services/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flickr
provider_slug: flickr
schemes:
- description: 'Flickr uses OAuth 1.0a (HMAC-SHA1). The OpenAPI 3 schema cannot model

    OAuth 1.0a directly, so this entry approximates the flow. Token URLs:

    - Request token: https://www.flickr.com/services/oauth/request_token

    - Authorize:     https://www.flickr.com/services/oauth/authorize

    - Access token:  https://www.flickr.com/services/oauth/access_token'
  flows:
  - authorizationUrl: https://www.flickr.com/services/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.flickr.com/services/oauth/access_token
  name: OAuth1
  source: openapi/flickr-openapi.yml
scope_count: 3
scope_names:
- delete
- read
- write
scopes:
- description: Delete content owned by the user
  flows:
  - authorizationCode
  scope: delete
- description: Read access to private content owned by the user
  flows:
  - authorizationCode
  scope: read
- description: Modify content owned by the user
  flows:
  - authorizationCode
  scope: write
slug: flickr-scopes
source_filename: flickr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flickr-openapi.yml\nschemes:\n- name: OAuth1\n  source: openapi/flickr-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.flickr.com/services/oauth/authorize\n    tokenUrl: https://www.flickr.com/services/oauth/access_token\n  description: |-\n    Flickr uses OAuth 1.0a (HMAC-SHA1). The OpenAPI 3 schema cannot model\n    OAuth 1.0a directly, so this entry approximates the flow. Token URLs:\n    - Request token: https://www.flickr.com/services/oauth/request_token\n    - Authorize:     https://www.flickr.com/services/oauth/authorize\n    - Access token:  https://www.flickr.com/services/oauth/access_token\nscopes:\n- scope: delete\n  description: Delete content owned by the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flickr-openapi.yml\n- scope: read\n  description: Read access to private content owned by the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flickr-openapi.yml\n\
  - scope: write\n  description: Modify content owned by the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flickr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flickr/refs/heads/main/scopes/flickr-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Photography
- Photos
- Social Media
- Public APIs
token_urls:
- https://www.flickr.com/services/oauth/access_token
---
