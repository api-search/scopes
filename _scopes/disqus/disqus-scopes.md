---
api_specs:
- filename: disqus-openapi.yml
  format: yaml
  label: Disqus Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/openapi/disqus-openapi.yml
authorization_urls:
- https://disqus.com/api/oauth/2.0/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Disqus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Disqus publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Disqus API on a user''s behalf.


  Tokens are issued from https://disqus.com/api/oauth/2.0/access_token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Disqus
provider_slug: disqus
schemes:
- flows:
  - authorizationUrl: https://disqus.com/api/oauth/2.0/authorize/
    flow: authorizationCode
    tokenUrl: https://disqus.com/api/oauth/2.0/access_token/
  name: oauth2
  source: openapi/disqus-openapi.yml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Forum administration
  flows:
  - authorizationCode
  scope: admin
- description: Read forums, threads, posts
  flows:
  - authorizationCode
  scope: read
- description: Create posts and threads
  flows:
  - authorizationCode
  scope: write
slug: disqus-scopes
source_filename: disqus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/disqus-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/disqus-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://disqus.com/api/oauth/2.0/authorize/\n    tokenUrl: https://disqus.com/api/oauth/2.0/access_token/\nscopes:\n- scope: admin\n  description: Forum administration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/disqus-openapi.yml\n- scope: read\n  description: Read forums, threads, posts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/disqus-openapi.yml\n- scope: write\n  description: Create posts and threads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/disqus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/scopes/disqus-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Comments
- Community
- Discussions
- Publishing
- Audience Engagement
- Social
token_urls:
- https://disqus.com/api/oauth/2.0/access_token/
---
