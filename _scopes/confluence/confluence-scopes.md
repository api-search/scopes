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
name: Confluence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Confluence publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Confluence API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Confluence
provider_slug: confluence
schemes:
- description: OAuth 2.0 (3LO) for Confluence Cloud apps.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuth2
  source: openapi/confluence-cloud-v2.yml
scope_count: 9
scope_names:
- delete:confluence-content
- read:confluence-content.all
- read:confluence-content.summary
- read:confluence-groups
- read:confluence-space.summary
- read:confluence-user
- write:confluence-content
- write:confluence-file
- write:confluence-space
scopes:
- description: Delete Confluence content
  flows:
  - authorizationCode
  scope: delete:confluence-content
- description: Read Confluence content
  flows:
  - authorizationCode
  scope: read:confluence-content.all
- description: Read Confluence content summaries
  flows:
  - authorizationCode
  scope: read:confluence-content.summary
- description: Read Confluence groups
  flows:
  - authorizationCode
  scope: read:confluence-groups
- description: Read Confluence space summaries
  flows:
  - authorizationCode
  scope: read:confluence-space.summary
- description: Read Confluence user information
  flows:
  - authorizationCode
  scope: read:confluence-user
- description: Create and update Confluence content
  flows:
  - authorizationCode
  scope: write:confluence-content
- description: Upload attachments to Confluence
  flows:
  - authorizationCode
  scope: write:confluence-file
- description: Create and update Confluence spaces
  flows:
  - authorizationCode
  scope: write:confluence-space
slug: confluence-scopes
source_filename: confluence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/confluence-cloud-v2.yml\nschemes:\n- name: oAuth2\n  source: openapi/confluence-cloud-v2.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth 2.0 (3LO) for Confluence Cloud apps.\nscopes:\n- scope: delete:confluence-content\n  description: Delete Confluence content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: read:confluence-content.all\n  description: Read Confluence content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: read:confluence-content.summary\n  description: Read Confluence content summaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: read:confluence-groups\n  description: Read Confluence groups\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/confluence-cloud-v2.yml\n- scope: read:confluence-space.summary\n  description: Read Confluence space summaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: read:confluence-user\n  description: Read Confluence user information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: write:confluence-content\n  description: Create and update Confluence content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: write:confluence-file\n  description: Upload attachments to Confluence\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- scope: write:confluence-space\n  description: Create and update Confluence spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/confluence-cloud-v2.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/scopes/confluence-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
token_urls:
- https://auth.atlassian.com/oauth/token
---
