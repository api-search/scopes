---
api_specs:
- filename: meta-openapi.yml
  format: yaml
  label: Facebook Graph API - User
  slug: facebook-graph-api-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/openapi/meta-openapi.yml
authorization_urls:
- https://www.facebook.com/v22.0/dialog/oauth
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Meta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meta publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meta API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meta
provider_slug: meta
schemes:
- flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: implicit
  name: userAccessToken
  source: openapi/meta-openapi.yml
scope_count: 1
scope_names:
- public_profile
scopes:
- description: Access basic profile info
  flows:
  - implicit
  scope: public_profile
slug: meta-scopes
source_filename: meta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meta-openapi.yml\nschemes:\n- name: userAccessToken\n  source: openapi/meta-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\nscopes:\n- scope: public_profile\n  description: Access basic profile info\n  flows:\n  - implicit\n  sources:\n  - openapi/meta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/scopes/meta-scopes.yml
summary_line: 1 scope · implicit
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
token_urls: []
---
