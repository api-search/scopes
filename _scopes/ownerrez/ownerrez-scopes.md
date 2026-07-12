---
authorization_urls:
- https://app.ownerrez.com/oauth/authorize
description: ''
docs: https://www.ownerrez.com/support/articles/api-oauth-app
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ownerrez Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OwnerRez publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OwnerRez API on a user''s behalf.


  Tokens are issued from https://api.ownerrez.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OwnerRez
provider_slug: ownerrez
schemes:
- description: OAuth 2.0 Authorization Code Grant (RFC 6749 Section 4.1). Register an OAuth app in the OwnerRez Developer/API settings, send the user to the authorization URL, then exchange the returned code for an access token.
  flows:
  - authorizationUrl: https://app.ownerrez.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.ownerrez.com/oauth/access_token
  name: oauth2
  source: openapi/ownerrez-openapi.yml
scope_count: 2
scope_names:
- full
- read
scopes:
- description: Full access to all API endpoints (read and write). Requested as scope=full on the authorization URL and returned as "scope":"full" in the access token response.
  flows: []
  scope: full
- description: Read-only access, limiting the token to GET endpoints only. Set via the OAuth app's "OAuth API scope" setting ("Read" instead of "Full"); a Read app cannot create read & write tokens later.
  flows: []
  scope: read
slug: ownerrez-scopes
source_filename: ownerrez-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/ownerrez-openapi.yml\ndocs: https://www.ownerrez.com/support/articles/api-oauth-app\nschemes:\n- name: oauth2\n  source: openapi/ownerrez-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.ownerrez.com/oauth/authorize\n    tokenUrl: https://api.ownerrez.com/oauth/access_token\n  description: OAuth 2.0 Authorization Code Grant (RFC 6749 Section 4.1). Register an OAuth\n    app in the OwnerRez Developer/API settings, send the user to the authorization URL, then\n    exchange the returned code for an access token.\nscopes:\n- scope: full\n  description: Full access to all API endpoints (read and write). Requested as scope=full\n    on the authorization URL and returned as \"scope\":\"full\" in the access token response.\n  sources:\n  - https://www.ownerrez.com/support/articles/api-oauth-app\n- scope: read\n  description: Read-only access, limiting the token to GET endpoints only. Set\
  \ via the OAuth\n    app's \"OAuth API scope\" setting (\"Read\" instead of \"Full\"); a Read app cannot create\n    read & write tokens later.\n  sources:\n  - https://www.ownerrez.com/support/articles/api-oauth-app\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/scopes/ownerrez-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Hospitality
- Bookings
- Channel Manager
token_urls:
- https://api.ownerrez.com/oauth/access_token
---
