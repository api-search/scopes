---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Wildapricot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WildApricot publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the WildApricot API on a user''s behalf.


  Tokens are issued from https://oauth.wildapricot.org/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WildApricot
provider_slug: wildapricot
schemes:
- description: OAuth2 authentication for WildApricot API
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.wildapricot.org/auth/token
  name: OAuth2
  source: openapi/wildapricot-admin-api-openapi.yml
scope_count: 1
scope_names:
- auto
scopes:
- description: Full API access
  flows:
  - clientCredentials
  scope: auto
slug: wildapricot-scopes
source_filename: wildapricot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wildapricot-admin-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/wildapricot-admin-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.wildapricot.org/auth/token\n  description: OAuth2 authentication for WildApricot API\nscopes:\n- scope: auto\n  description: Full API access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/wildapricot-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/scopes/wildapricot-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Membership Management
- Associations
- Nonprofit
- Events
- Payments
token_urls:
- https://oauth.wildapricot.org/auth/token
---
