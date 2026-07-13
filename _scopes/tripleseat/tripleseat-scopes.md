---
api_specs:
- filename: tripleseat-openapi.yml
  format: yaml
  label: Tripleseat API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-openapi.yml
authorization_urls:
- https://api.tripleseat.com/oauth/authorize
description: ''
docs: https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tripleseat Scopes
name_suffix: OAuth Scopes
note: Tripleseat OAuth 2.0 applications request the coarse read and write scopes in the authorization flow; the migration guide's token exchange example also shows granular per-resource scopes (events:read, events:write, leads:read, leads:write, ...) determined by the OAuth 2.0 application's configuration, but no exhaustive list of the granular scopes is published.
overview: 'Tripleseat publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tripleseat API on a user''s behalf.


  Tokens are issued from https://api.tripleseat.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tripleseat
provider_slug: tripleseat
schemes:
- description: OAuth 2.0. Access tokens are Bearer tokens that expire after 7200 seconds (2 hours) and are accompanied by a refresh token. OAuth 1.0 is deprecated and discontinued on July 1, 2026.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.tripleseat.com/oauth/token
  - authorizationUrl: https://api.tripleseat.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.tripleseat.com/oauth/token
  name: oauth2
  source: openapi/tripleseat-openapi.yml
scope_count: 6
scope_names:
- read
- write
- events:read
- events:write
- leads:read
- leads:write
scopes:
- description: Read access to the Tripleseat API; requested in the documented OAuth 2.0 authorization flow (scope=read write) and returned in token responses.
  flows: []
  scope: read
- description: Write access to the Tripleseat API; requested in the documented OAuth 2.0 authorization flow (scope=read write) and returned in token responses.
  flows: []
  scope: write
- description: Granular read scope for events, shown in the OAuth 1.0-to-2.0 token exchange example response; returned scopes are determined by the OAuth 2.0 application's configuration.
  flows: []
  scope: events:read
- description: Granular write scope for events, shown in the OAuth 1.0-to-2.0 token exchange example response; returned scopes are determined by the OAuth 2.0 application's configuration.
  flows: []
  scope: events:write
- description: Granular read scope for leads, shown in the OAuth 1.0-to-2.0 token exchange example response; returned scopes are determined by the OAuth 2.0 application's configuration.
  flows: []
  scope: leads:read
- description: Granular write scope for leads, shown in the OAuth 1.0-to-2.0 token exchange example response; returned scopes are determined by the OAuth 2.0 application's configuration.
  flows: []
  scope: leads:write
slug: tripleseat-scopes
source_filename: tripleseat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/tripleseat-openapi.yml\ndocs: https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication\nnote: Tripleseat OAuth 2.0 applications request the coarse read and write scopes in\n  the authorization flow; the migration guide's token exchange example also shows\n  granular per-resource scopes (events:read, events:write, leads:read, leads:write,\n  ...) determined by the OAuth 2.0 application's configuration, but no exhaustive\n  list of the granular scopes is published.\nschemes:\n- name: oauth2\n  source: openapi/tripleseat-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.tripleseat.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.tripleseat.com/oauth/authorize\n    tokenUrl: https://api.tripleseat.com/oauth/token\n  description: OAuth 2.0. Access tokens are Bearer tokens that expire after 7200 seconds (2\n    hours) and are accompanied\
  \ by a refresh token. OAuth 1.0 is deprecated and discontinued\n    on July 1, 2026.\nscopes:\n- scope: read\n  description: Read access to the Tripleseat API; requested in the documented OAuth\n    2.0 authorization flow (scope=read write) and returned in token responses.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n- scope: write\n  description: Write access to the Tripleseat API; requested in the documented OAuth\n    2.0 authorization flow (scope=read write) and returned in token responses.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n- scope: events:read\n  description: Granular read scope for events, shown in the OAuth 1.0-to-2.0\
  \ token\n    exchange example response; returned scopes are determined by the OAuth 2.0\n    application's configuration.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n- scope: events:write\n  description: Granular write scope for events, shown in the OAuth 1.0-to-2.0 token\n    exchange example response; returned scopes are determined by the OAuth 2.0\n    application's configuration.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n- scope: leads:read\n  description: Granular read scope for leads, shown in the OAuth 1.0-to-2.0 token\n    exchange example response; returned scopes are determined by the OAuth 2.0\n    application's configuration.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n- scope: leads:write\n\
  \  description: Granular write scope for leads, shown in the OAuth 1.0-to-2.0 token\n    exchange example response; returned scopes are determined by the OAuth 2.0\n    application's configuration.\n  sources:\n  - https://support.tripleseat.com/hc/en-us/articles/35211389645079-OAuth-1-0-to-OAuth-2-0-Migration-Guide-for-Tripleseat-API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/scopes/tripleseat-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- Restaurant
- Events
- Catering
- Leads
- Webhooks
- Sales
token_urls:
- https://api.tripleseat.com/oauth/token
---
