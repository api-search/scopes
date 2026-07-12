---
authorization_urls:
- https://accounts.shutterstock.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Shutterstock Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shutterstock publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shutterstock API on a user''s behalf.


  Tokens are issued from https://api.shutterstock.com/v2/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shutterstock
provider_slug: shutterstock
schemes:
- flows:
  - authorizationUrl: https://accounts.shutterstock.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.shutterstock.com/v2/oauth/access_token
  name: customer_accessCode
  source: openapi/shutterstock-openapi.yml
scope_count: 6
scope_names:
- collections.edit
- collections.view
- licenses.create
- licenses.view
- purchases.view
- user.view
scopes:
- description: Grant the ability to create new collections, edit a collection, and modify the contents of a collection
  flows:
  - authorizationCode
  scope: collections.edit
- description: Grant read-only access to a collection and its contents.
  flows:
  - authorizationCode
  scope: collections.view
- description: Grant the ability to download and license media on behalf of the user.
  flows:
  - authorizationCode
  scope: licenses.create
- description: Grant read-only access to a user's licenses.
  flows:
  - authorizationCode
  scope: licenses.view
- description: Grant read-only access to a user's purchase history.
  flows:
  - authorizationCode
  scope: purchases.view
- description: ''
  flows: []
  scope: user.view
slug: shutterstock-scopes
source_filename: shutterstock-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shutterstock-openapi.yml\nschemes:\n- name: customer_accessCode\n  source: openapi/shutterstock-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.shutterstock.com/oauth/authorize\n    tokenUrl: https://api.shutterstock.com/v2/oauth/access_token\nscopes:\n- scope: collections.edit\n  description: Grant the ability to create new collections, edit a collection, and modify the\n    contents of a collection\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shutterstock-openapi.yml\n- scope: collections.view\n  description: Grant read-only access to a collection and its contents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shutterstock-openapi.yml\n- scope: licenses.create\n  description: Grant the ability to download and license media on behalf of the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shutterstock-openapi.yml\n- scope: licenses.view\n\
  \  description: Grant read-only access to a user's licenses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shutterstock-openapi.yml\n- scope: purchases.view\n  description: Grant read-only access to a user's purchase history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shutterstock-openapi.yml\n- scope: user.view\n  sources:\n  - openapi/shutterstock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shutterstock/refs/heads/main/scopes/shutterstock-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Images
- Media
- Photos
- Stock Images
- Videos
- Audio
- Licensing
- Creative Content
token_urls:
- https://api.shutterstock.com/v2/oauth/access_token
---
