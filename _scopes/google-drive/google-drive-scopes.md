---
api_specs:
- filename: google-drive-openapi.yml
  format: yaml
  label: Google Drive API v3
  slug: google-drive-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/openapi/google-drive-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: 'OAuth 2.0 scopes for the Google Drive API v3. The captured OpenAPI does not declare securitySchemes, so the derive pass yields nothing; these scopes were read from Google''s Drive API-specific authorization reference and grouped by Google''s sensitivity tier (non-sensitive / sensitive / restricted). Restricted scopes require a Google security assessment before production use. Authorization server: accounts.google.com (see well-known/google-drive-openid-configuration.json).'
docs: https://developers.google.com/workspace/drive/api/guides/api-specific-auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Drive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Drive publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Drive API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Drive
provider_slug: google-drive
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: docs
  type: oauth2
scope_count: 13
scope_names:
- https://www.googleapis.com/auth/drive
- https://www.googleapis.com/auth/drive.readonly
- https://www.googleapis.com/auth/drive.file
- https://www.googleapis.com/auth/drive.appdata
- https://www.googleapis.com/auth/drive.appfolder
- https://www.googleapis.com/auth/drive.install
- https://www.googleapis.com/auth/drive.metadata
- https://www.googleapis.com/auth/drive.metadata.readonly
- https://www.googleapis.com/auth/drive.apps.readonly
- https://www.googleapis.com/auth/drive.activity
- https://www.googleapis.com/auth/drive.activity.readonly
- https://www.googleapis.com/auth/drive.meet.readonly
- https://www.googleapis.com/auth/drive.scripts
scopes:
- description: View and manage all of a user's Drive files.
  flows: []
  scope: https://www.googleapis.com/auth/drive
- description: View and download all of a user's Drive files.
  flows: []
  scope: https://www.googleapis.com/auth/drive.readonly
- description: Create new Drive files, or view/modify files created or opened by the app (per-file access).
  flows: []
  scope: https://www.googleapis.com/auth/drive.file
- description: View and manage the app's own hidden application-data folder.
  flows: []
  scope: https://www.googleapis.com/auth/drive.appdata
- description: View and manage the app's own hidden application-data folder.
  flows: []
  scope: https://www.googleapis.com/auth/drive.appfolder
- description: Allow the app to appear in the "Open with" or "New" menu.
  flows: []
  scope: https://www.googleapis.com/auth/drive.install
- description: View and manage metadata of files in the user's Drive.
  flows: []
  scope: https://www.googleapis.com/auth/drive.metadata
- description: View metadata for files in the user's Drive.
  flows: []
  scope: https://www.googleapis.com/auth/drive.metadata.readonly
- description: View apps authorized to access the user's Drive.
  flows: []
  scope: https://www.googleapis.com/auth/drive.apps.readonly
- description: View and add to the activity record of files in the user's Drive.
  flows: []
  scope: https://www.googleapis.com/auth/drive.activity
- description: View the activity record of files in the user's Drive.
  flows: []
  scope: https://www.googleapis.com/auth/drive.activity.readonly
- description: View Drive files created or edited by Google Meet.
  flows: []
  scope: https://www.googleapis.com/auth/drive.meet.readonly
- description: Modify the behavior of the user's Google Apps Script scripts.
  flows: []
  scope: https://www.googleapis.com/auth/drive.scripts
slug: google-drive-scopes
source_filename: google-drive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-drive-openapi.yml\ndocs: https://developers.google.com/workspace/drive/api/guides/api-specific-auth\ndescription: >-\n  OAuth 2.0 scopes for the Google Drive API v3. The captured OpenAPI does not\n  declare securitySchemes, so the derive pass yields nothing; these scopes were\n  read from Google's Drive API-specific authorization reference and grouped by\n  Google's sensitivity tier (non-sensitive / sensitive / restricted). Restricted\n  scopes require a Google security assessment before production use. Authorization\n  server: accounts.google.com (see well-known/google-drive-openid-configuration.json).\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: docs\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n  - scope: https://www.googleapis.com/auth/drive\n    tier: restricted\n\
  \    description: View and manage all of a user's Drive files.\n  - scope: https://www.googleapis.com/auth/drive.readonly\n    tier: restricted\n    description: View and download all of a user's Drive files.\n  - scope: https://www.googleapis.com/auth/drive.file\n    tier: non-sensitive\n    description: Create new Drive files, or view/modify files created or opened by the app (per-file access).\n  - scope: https://www.googleapis.com/auth/drive.appdata\n    tier: non-sensitive\n    description: View and manage the app's own hidden application-data folder.\n  - scope: https://www.googleapis.com/auth/drive.appfolder\n    tier: non-sensitive\n    description: View and manage the app's own hidden application-data folder.\n  - scope: https://www.googleapis.com/auth/drive.install\n    tier: non-sensitive\n    description: Allow the app to appear in the \"Open with\" or \"New\" menu.\n  - scope: https://www.googleapis.com/auth/drive.metadata\n    tier: restricted\n    description: View and manage\
  \ metadata of files in the user's Drive.\n  - scope: https://www.googleapis.com/auth/drive.metadata.readonly\n    tier: restricted\n    description: View metadata for files in the user's Drive.\n  - scope: https://www.googleapis.com/auth/drive.apps.readonly\n    tier: sensitive\n    description: View apps authorized to access the user's Drive.\n  - scope: https://www.googleapis.com/auth/drive.activity\n    tier: restricted\n    description: View and add to the activity record of files in the user's Drive.\n  - scope: https://www.googleapis.com/auth/drive.activity.readonly\n    tier: restricted\n    description: View the activity record of files in the user's Drive.\n  - scope: https://www.googleapis.com/auth/drive.meet.readonly\n    tier: restricted\n    description: View Drive files created or edited by Google Meet.\n  - scope: https://www.googleapis.com/auth/drive.scripts\n    tier: restricted\n    description: Modify the behavior of the user's Google Apps Script scripts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/scopes/google-drive-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drive
- Files
- Google
- Storage
token_urls:
- https://oauth2.googleapis.com/token
---
