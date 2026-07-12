---
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Atlassian Confluence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Atlassian Confluence publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Atlassian Confluence API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atlassian Confluence
provider_slug: atlassian-confluence
schemes:
- description: OAuth 2.0 (3LO) for Atlassian Cloud Connect/Forge apps
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  source: openapi/atlassian-confluence-openapi.yml
scope_count: 7
scope_names:
- read:confluence-content.all
- read:confluence-content.summary
- read:page:confluence
- read:space:confluence
- write:confluence-content
- write:page:confluence
- write:space:confluence
scopes:
- description: Read full content
  flows:
  - authorizationCode
  scope: read:confluence-content.all
- description: Read content summaries
  flows:
  - authorizationCode
  scope: read:confluence-content.summary
- description: Read pages (v2)
  flows:
  - authorizationCode
  scope: read:page:confluence
- description: Read spaces (v2)
  flows:
  - authorizationCode
  scope: read:space:confluence
- description: Create, update, and delete content
  flows:
  - authorizationCode
  scope: write:confluence-content
- description: Create and update pages (v2)
  flows:
  - authorizationCode
  scope: write:page:confluence
- description: Create and update spaces (v2)
  flows:
  - authorizationCode
  scope: write:space:confluence
slug: atlassian-confluence-scopes
source_filename: atlassian-confluence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-confluence-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/atlassian-confluence-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 (3LO) for Atlassian Cloud Connect/Forge apps\nscopes:\n- scope: read:confluence-content.all\n  description: Read full content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: read:confluence-content.summary\n  description: Read content summaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: read:page:confluence\n  description: Read pages (v2)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: read:space:confluence\n  description: Read spaces (v2)\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: write:confluence-content\n  description: Create, update, and delete content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: write:page:confluence\n  description: Create and update pages (v2)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- scope: write:space:confluence\n  description: Create and update spaces (v2)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/scopes/atlassian-confluence-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Atlassian
- Collaboration
- Content Management
- Documentation
- Knowledge Management
- Wiki
token_urls:
- https://auth.atlassian.com/oauth/token
---
