---
authorization_urls: []
description: ''
docs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Grubhub Scopes
name_suffix: OAuth Scopes
note: Grubhub's partner Onboarding/Menu/Orders APIs use OAuth client credentials without published named scopes; the only documented scope values ("anonymous" and "openid diner") appear in the Grubhub Developers Open ID Authentication guide for diner-facing ordering integrations.
overview: 'grubhub publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the grubhub API on a user''s behalf.


  Tokens are issued from /oauth2/direct/auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: grubhub
provider_slug: grubhub
schemes:
- description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate merchant onboarding operations.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/direct/auth
  name: oauthAuth
  source: openapi/grubhub-onboarding-openapi.yml
scope_count: 2
scope_names:
- anonymous
- openid diner
scopes:
- description: Anonymous authentication via POST /oauth2/direct/auth (grant_type token). Returns an access token that can be used to browse restaurant information and begin an order without a logged-in diner; any call except checkout is permitted until the session is connected to an authenticated diner.
  flows: []
  scope: anonymous
- description: Required scope value when authenticating a diner via POST /oauth2/direct/auth with a signed OpenID token (grant_type token). Links the partner application's user to a Grubhub diner record and returns an access token for making Grubhub API calls on that diner's behalf, including checkout.
  flows: []
  scope: openid diner
slug: grubhub-scopes
source_filename: grubhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/grubhub-onboarding-openapi.yml\ndocs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\nschemes:\n- name: oauthAuth\n  source: openapi/grubhub-onboarding-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/direct/auth\n  description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate\n    merchant onboarding operations.\nscopes:\n- scope: anonymous\n  description: Anonymous authentication via POST /oauth2/direct/auth (grant_type token). Returns\n    an access token that can be used to browse restaurant information and begin an order without\n    a logged-in diner; any call except checkout is permitted until the session is connected to\n    an authenticated diner.\n  sources:\n  - https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\n- scope: openid diner\n  description: Required\
  \ scope value when authenticating a diner via POST /oauth2/direct/auth with\n    a signed OpenID token (grant_type token). Links the partner application's user to a Grubhub\n    diner record and returns an access token for making Grubhub API calls on that diner's behalf,\n    including checkout.\n  sources:\n  - https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\nnote: Grubhub's partner Onboarding/Menu/Orders APIs use OAuth client credentials without published\n  named scopes; the only documented scope values (\"anonymous\" and \"openid diner\") appear in the\n  Grubhub Developers Open ID Authentication guide for diner-facing ordering integrations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/scopes/grubhub-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- /oauth2/direct/auth
---
