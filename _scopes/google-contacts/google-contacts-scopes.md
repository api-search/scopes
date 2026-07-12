---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Contacts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google People API publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google People API API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google People API
provider_slug: google-contacts
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/contacts.yml
scope_count: 4
scope_names:
- https://www.googleapis.com/auth/contacts
- https://www.googleapis.com/auth/contacts.other.readonly
- https://www.googleapis.com/auth/contacts.readonly
- https://www.googleapis.com/auth/directory.readonly
scopes:
- description: See, edit, download, and permanently delete your contacts
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts
- description: See and download contact info automatically saved in your Other contacts
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts.other.readonly
- description: See and download your contacts
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts.readonly
- description: See and download your organization's GSuite directory
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/directory.readonly
slug: google-contacts-scopes
source_filename: google-contacts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contacts.yml\nschemes:\n- name: oauth2\n  source: openapi/contacts.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/contacts\n  description: See, edit, download, and permanently delete your contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contacts.yml\n- scope: https://www.googleapis.com/auth/contacts.other.readonly\n  description: See and download contact info automatically saved in your Other contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contacts.yml\n- scope: https://www.googleapis.com/auth/contacts.readonly\n  description: See and download your contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contacts.yml\n- scope: https://www.googleapis.com/auth/directory.readonly\n  description: See and download your\
  \ organization's GSuite directory\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/contacts.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/scopes/google-contacts-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Address Book
- Contacts
- Directory
- Google
- People
- Profiles
token_urls:
- https://oauth2.googleapis.com/token
---
