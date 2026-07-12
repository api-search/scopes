---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Google Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google publishes 18 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google
provider_slug: google
schemes:
- description: OAuth 2.0 authentication for Google Books API
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/books-api-openapi.yml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-docs-api-openapi.yml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-docs-api-openapi.yml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-drive-activity-api-openapi.yml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-drive-activity-api-openapi.yml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-drive-api-openapi.yml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-drive-api-openapi.yml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-drive-labels-api-openapi.yml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-drive-labels-api-openapi.yml
scope_count: 18
scope_names:
- https://www.googleapis.com/auth/books
- https://www.googleapis.com/auth/documents
- https://www.googleapis.com/auth/documents.readonly
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.activity
- https://www.googleapis.com/auth/drive.activity.readonly
- https://www.googleapis.com/auth/drive.admin.labels
- https://www.googleapis.com/auth/drive.admin.labels.readonly
- https://www.googleapis.com/auth/drive.appdata
- https://www.googleapis.com/auth/drive.apps.readonly
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.labels
- https://www.googleapis.com/auth/drive.labels.readonly
- https://www.googleapis.com/auth/drive.metadata
- https://www.googleapis.com/auth/drive.metadata.readonly
- https://www.googleapis.com/auth/drive.photos.readonly
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/drive.scripts
scopes:
- description: Manage your Google Books library
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/books
- description: See, edit, create, and delete all your Google Docs documents
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/documents
- description: See all your Google Docs documents
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/documents.readonly
- description: See, edit, create, and delete all of your Google Drive files
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive
- description: View and add to the activity record of files in your Google Drive
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.activity
- description: View the activity record of files in your Google Drive
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.activity.readonly
- description: See, edit, create, and delete all Google Drive labels in your organization, and see your organization's label-related admin policies
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.admin.labels
- description: See all Google Drive labels and label-related admin policies in your organization
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.admin.labels.readonly
- description: See, create, and delete its own configuration data in your Google Drive
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.appdata
- description: View your Google Drive apps
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.apps.readonly
- description: See, edit, create, and delete only the specific Google Drive files you use with this app
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.file
- description: See, edit, create, and delete your Google Drive labels
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.labels
- description: See your Google Drive labels
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.labels.readonly
- description: View and manage metadata of files in your Google Drive
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.metadata
- description: See information about your Google Drive files
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.metadata.readonly
- description: View the photos, videos and albums in your Google Photos
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.photos.readonly
- description: See and download all your Google Drive files
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.readonly
- description: Modify your Google Apps Script scripts' behavior
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/drive.scripts
slug: google-scopes
source_filename: google-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/books-api-openapi.yml, openapi/google-docs-api-openapi.yml, openapi/google-drive-activity-api-openapi.yml,\n  openapi/google-drive-api-openapi.yml, openapi/google-drive-labels-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/books-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for Google Books API\n- name: Oauth2\n  source: openapi/google-docs-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-docs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth\
  \ 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-drive-activity-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-drive-activity-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-drive-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-drive-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description:\
  \ Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-drive-labels-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-drive-labels-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\nscopes:\n- scope: https://www.googleapis.com/auth/books\n  description: Manage your Google Books library\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/books-api-openapi.yml\n- scope: https://www.googleapis.com/auth/documents\n  description: See, edit, create, and delete all your Google Docs documents\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-docs-api-openapi.yml\n- scope: https://www.googleapis.com/auth/documents.readonly\n\
  \  description: See all your Google Docs documents\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-docs-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive\n  description: See, edit, create, and delete all of your Google Drive files\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-docs-api-openapi.yml\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.activity\n  description: View and add to the activity record of files in your Google Drive\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-activity-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.activity.readonly\n  description: View the activity record of files in your Google Drive\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-activity-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.admin.labels\n  description: See, edit,\
  \ create, and delete all Google Drive labels in your organization, and\n    see your organization's label-related admin policies\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-labels-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.admin.labels.readonly\n  description: See all Google Drive labels and label-related admin policies in your organization\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-labels-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.appdata\n  description: See, create, and delete its own configuration data in your Google Drive\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.apps.readonly\n  description: View your Google Drive apps\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.file\n\
  \  description: See, edit, create, and delete only the specific Google Drive files you use with\n    this app\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-docs-api-openapi.yml\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.labels\n  description: See, edit, create, and delete your Google Drive labels\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-labels-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.labels.readonly\n  description: See your Google Drive labels\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-labels-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.metadata\n  description: View and manage metadata of files in your Google Drive\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.metadata.readonly\n\
  \  description: See information about your Google Drive files\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.photos.readonly\n  description: View the photos, videos and albums in your Google Photos\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.readonly\n  description: See and download all your Google Drive files\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-docs-api-openapi.yml\n  - openapi/google-drive-api-openapi.yml\n- scope: https://www.googleapis.com/auth/drive.scripts\n  description: Modify your Google Apps Script scripts' behavior\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-drive-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/scopes/google-scopes.yml
summary_line: 18 scopes · authorizationCode/implicit
tags:
- Advertising
- Cloud
- Developer
- Google
- Platform
- Search
- T1
token_urls:
- https://oauth2.googleapis.com/token
- https://accounts.google.com/o/oauth2/token
---
