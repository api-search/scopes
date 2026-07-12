---
authorization_urls: []
description: ''
docs: https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Podbean Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Podbean API publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Podbean API API on a user''s behalf.


  Tokens are issued from https://api.podbean.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Podbean API
provider_slug: podbean-api
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.podbean.com/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/podbean-api-openapi.yml
scope_count: 5
scope_names:
- podcast_read
- podcast_update
- episode_read
- episode_publish
- private_members
scopes:
- description: Read podcast
  flows: []
  scope: podcast_read
- description: Update podcast
  flows: []
  scope: podcast_update
- description: Read episode
  flows: []
  scope: episode_read
- description: Create/Update/Delete episode
  flows: []
  scope: episode_publish
- description: Create/Read/Update/Delete private members (only available to Business Master Account with Client Credentials authentication)
  flows: []
  scope: private_members
slug: podbean-api-scopes
source_filename: podbean-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/podbean-api-openapi.yml\ndocs: https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/podbean-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.podbean.com/v1/oauth/token\nscopes:\n- scope: podcast_read\n  description: Read podcast\n  sources:\n  - https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\n- scope: podcast_update\n  description: Update podcast\n  sources:\n  - https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\n- scope: episode_read\n  description: Read episode\n  sources:\n  - https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\n- scope: episode_publish\n  description: Create/Update/Delete episode\n  sources:\n  - https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\n- scope: private_members\n  description:\
  \ Create/Read/Update/Delete private members (only available to Business\n    Master Account with Client Credentials authentication)\n  sources:\n  - https://developers.podbean.com/podbean-api-docs/#api-appendix-permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean-api/refs/heads/main/scopes/podbean-api-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Podcasts
- Podcasting
- Audio
- Media
- OAuth
- Episodes
token_urls:
- https://api.podbean.com/v1/oauth/token
---
