---
api_specs:
- filename: google-books-volumes-api-openapi.yml
  format: yaml
  label: Google Books Volumes API
  slug: google-books-volumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-volumes-api-openapi.yml
- filename: google-books-bookshelves-api-openapi.yml
  format: yaml
  label: Google Books Bookshelves API
  slug: google-books-bookshelves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-bookshelves-api-openapi.yml
- filename: google-books-cloudloading-api-openapi.yml
  format: yaml
  label: Google Books Cloudloading API
  slug: google-books-cloudloading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-cloudloading-api-openapi.yml
- filename: google-books-dictionary-api-openapi.yml
  format: yaml
  label: Google Books Dictionary API
  slug: google-books-dictionary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-dictionary-api-openapi.yml
- filename: google-books-familysharing-api-openapi.yml
  format: yaml
  label: Google Books Familysharing API
  slug: google-books-familysharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-familysharing-api-openapi.yml
- filename: google-books-layers-api-openapi.yml
  format: yaml
  label: Google Books Layers API
  slug: google-books-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-layers-api-openapi.yml
- filename: google-books-myconfig-api-openapi.yml
  format: yaml
  label: Google Books Myconfig API
  slug: google-books-myconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-myconfig-api-openapi.yml
- filename: google-books-notification-api-openapi.yml
  format: yaml
  label: Google Books Notification API
  slug: google-books-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-notification-api-openapi.yml
- filename: google-books-onboarding-api-openapi.yml
  format: yaml
  label: Google Books Onboarding API
  slug: google-books-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-onboarding-api-openapi.yml
- filename: google-books-personalizedstream-api-openapi.yml
  format: yaml
  label: Google Books Personalizedstream API
  slug: google-books-personalizedstream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-personalizedstream-api-openapi.yml
- filename: google-books-promooffer-api-openapi.yml
  format: yaml
  label: Google Books Promooffer API
  slug: google-books-promooffer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-promooffer-api-openapi.yml
- filename: google-books-series-api-openapi.yml
  format: yaml
  label: Google Books Series API
  slug: google-books-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-series-api-openapi.yml
- filename: google-books-mylibrary-api-openapi.yml
  format: yaml
  label: Google Books Books Mylibrary API
  slug: google-books-mylibrary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-mylibrary-api-openapi.yml
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
source_yaml_url: https://artifacts.apis.io/google-books/scopes/google-books-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Books
- Ebooks
- Google
- Library
- Publishing
- Reading
- Search
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
