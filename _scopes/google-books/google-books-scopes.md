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
name: Google Books Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Books publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Books API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Books
provider_slug: google-books
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/books.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/books
scopes:
- description: Manage your books
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/books
slug: google-books-scopes
source_filename: google-books-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/books.yml\nschemes:\n- name: oauth2\n  source: openapi/books.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/books\n  description: Manage your books\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/books.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-books/refs/heads/main/scopes/google-books-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Books
- eBooks
- Google
- Library
- Publishing
- Reading
- Search
token_urls:
- https://oauth2.googleapis.com/token
---
