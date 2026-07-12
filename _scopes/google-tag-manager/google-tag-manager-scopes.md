---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Tag Manager Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Tag Manager publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Tag Manager API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schemes:
- description: OAuth 2.0 authentication for Google Tag Manager API.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-tag-manager-api-v2-openapi.yml
scope_count: 7
scope_names:
- tagmanager.delete.containers
- tagmanager.edit.containers
- tagmanager.edit.containerversions
- tagmanager.manage.accounts
- tagmanager.manage.users
- tagmanager.publish
- tagmanager.readonly
scopes:
- description: Delete your Google Tag Manager containers.
  flows:
  - authorizationCode
  scope: tagmanager.delete.containers
- description: Manage your Google Tag Manager container and its subcomponents, excluding versioning and publishing.
  flows:
  - authorizationCode
  scope: tagmanager.edit.containers
- description: Manage your Google Tag Manager container versions.
  flows:
  - authorizationCode
  scope: tagmanager.edit.containerversions
- description: View and manage your Google Tag Manager accounts.
  flows:
  - authorizationCode
  scope: tagmanager.manage.accounts
- description: Manage user permissions of your Google Tag Manager account and container.
  flows:
  - authorizationCode
  scope: tagmanager.manage.users
- description: Publish your Google Tag Manager container versions.
  flows:
  - authorizationCode
  scope: tagmanager.publish
- description: View your Google Tag Manager container and its subcomponents.
  flows:
  - authorizationCode
  scope: tagmanager.readonly
slug: google-tag-manager-scopes
source_filename: google-tag-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-tag-manager-api-v2-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-tag-manager-api-v2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google Tag Manager API.\nscopes:\n- scope: tagmanager.delete.containers\n  description: Delete your Google Tag Manager containers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.edit.containers\n  description: Manage your Google Tag Manager container and its subcomponents, excluding versioning\n    and publishing.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.edit.containerversions\n  description: Manage your Google Tag Manager container versions.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.manage.accounts\n  description: View and manage your Google Tag Manager accounts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.manage.users\n  description: Manage user permissions of your Google Tag Manager account and container.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.publish\n  description: Publish your Google Tag Manager container versions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n- scope: tagmanager.readonly\n  description: View your Google Tag Manager container and its subcomponents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/scopes/google-tag-manager-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
token_urls:
- https://oauth2.googleapis.com/token
---
