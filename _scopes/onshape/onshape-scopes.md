---
api_specs:
- filename: onshape-openapi-original.json
  format: json
  label: Onshape REST API
  slug: onshape-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/openapi/onshape-openapi-original.json
authorization_urls:
- /oauth/authorize
description: ''
docs: https://onshape-public.github.io/docs/auth/oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Onshape Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Onshape publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Onshape API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Onshape
provider_slug: onshape
schemes:
- description: Use OAuth 2.0 to authenticate requests.
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/onshape-openapi-original.json
scope_count: 24
scope_names:
- OAuth2Delete
- OAuth2Internal
- OAuth2Purchase
- OAuth2Read
- OAuth2ReadPII
- OAuth2Share
- OAuth2Write
- PLMIntegration
- document.create
- document.delete
- document.edit
- document.read
- enterprise.create
- enterprise.delete
- enterprise.edit
- enterprise.member.create
- enterprise.member.delete
- enterprise.member.edit
- enterprise.member.read
- enterprise.read
- webhook.create
- webhook.delete
- webhook.edit
- webhook.read
scopes:
- description: Application can delete your documents and workspaces
  flows:
  - authorizationCode
  scope: OAuth2Delete
- description: Application is Onshape Internal
  flows:
  - authorizationCode
  scope: OAuth2Internal
- description: Application can request purchases on your behalf
  flows:
  - authorizationCode
  scope: OAuth2Purchase
- description: Application can read your documents
  flows:
  - authorizationCode
  scope: OAuth2Read
- description: Application can read your profile information
  flows:
  - authorizationCode
  scope: OAuth2ReadPII
- description: Application can share and unshare documents on your behalf
  flows:
  - authorizationCode
  scope: OAuth2Share
- description: Application can write to your documents
  flows:
  - authorizationCode
  scope: OAuth2Write
- description: PLM automation can invoke limited operations
  flows:
  - authorizationCode
  scope: PLMIntegration
- description: Atlas Application can create a document
  flows:
  - authorizationCode
  scope: document.create
- description: Atlas Application can delete a document
  flows:
  - authorizationCode
  scope: document.delete
- description: Atlas Application can edit a document
  flows:
  - authorizationCode
  scope: document.edit
- description: Atlas Application can read a document
  flows:
  - authorizationCode
  scope: document.read
- description: Atlas Application can create an enterprise
  flows:
  - authorizationCode
  scope: enterprise.create
- description: Atlas Application can delete an enterprise
  flows:
  - authorizationCode
  scope: enterprise.delete
- description: Atlas Application can edit an enterprise
  flows:
  - authorizationCode
  scope: enterprise.edit
- description: Atlas Application can create an enterprise member
  flows:
  - authorizationCode
  scope: enterprise.member.create
- description: Atlas Application can delete a member from an enterprise
  flows:
  - authorizationCode
  scope: enterprise.member.delete
- description: Atlas Application can edit the details of an enterprise member
  flows:
  - authorizationCode
  scope: enterprise.member.edit
- description: Atlas Application can read the details of an enterprise member
  flows:
  - authorizationCode
  scope: enterprise.member.read
- description: Atlas Application can read from an enterprise
  flows:
  - authorizationCode
  scope: enterprise.read
- description: Atlas Application can create a webhook on behalf of the logged-in user
  flows:
  - authorizationCode
  scope: webhook.create
- description: Atlas Application can delete a webhook on behalf of the logged-in user
  flows:
  - authorizationCode
  scope: webhook.delete
- description: Atlas Application can edit a webhook on behalf of the logged-in user
  flows:
  - authorizationCode
  scope: webhook.edit
- description: Atlas Application can read a webhook on behalf of the logged-in user
  flows:
  - authorizationCode
  scope: webhook.read
slug: onshape-scopes
source_filename: onshape-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/onshape-openapi-original.json\ndocs: https://onshape-public.github.io/docs/auth/oauth/\nschemes:\n- name: OAuth2\n  source: openapi/onshape-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  description: Use OAuth 2.0 to authenticate requests.\nscopes:\n- scope: OAuth2Delete\n  description: Application can delete your documents and workspaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2Internal\n  description: Application is Onshape Internal\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2Purchase\n  description: Application can request purchases on your behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2Read\n  description: Application can read your documents\n \
  \ flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2ReadPII\n  description: Application can read your profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2Share\n  description: Application can share and unshare documents on your behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: OAuth2Write\n  description: Application can write to your documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: PLMIntegration\n  description: PLM automation can invoke limited operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: document.create\n  description: Atlas Application can create a document\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: document.delete\n  description: Atlas\
  \ Application can delete a document\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: document.edit\n  description: Atlas Application can edit a document\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: document.read\n  description: Atlas Application can read a document\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.create\n  description: Atlas Application can create an enterprise\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.delete\n  description: Atlas Application can delete an enterprise\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.edit\n  description: Atlas Application can edit an enterprise\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.member.create\n\
  \  description: Atlas Application can create an enterprise member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.member.delete\n  description: Atlas Application can delete a member from an enterprise\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.member.edit\n  description: Atlas Application can edit the details of an enterprise member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.member.read\n  description: Atlas Application can read the details of an enterprise member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: enterprise.read\n  description: Atlas Application can read from an enterprise\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: webhook.create\n  description: Atlas Application can create a webhook\
  \ on behalf of the logged-in user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: webhook.delete\n  description: Atlas Application can delete a webhook on behalf of the logged-in user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: webhook.edit\n  description: Atlas Application can edit a webhook on behalf of the logged-in user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n- scope: webhook.read\n  description: Atlas Application can read a webhook on behalf of the logged-in user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/onshape-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onshape/refs/heads/main/scopes/onshape-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Company
- CAD
- PLM
- Product Data Management
- Engineering
- Manufacturing
- Design
- Cloud
- Developer Tools
token_urls:
- /oauth/token
---
