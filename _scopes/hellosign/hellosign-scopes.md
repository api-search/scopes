---
api_specs:
- filename: hellosign-openapi-original.yaml
  format: yaml
  label: Dropbox Sign API
  slug: dropbox-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-openapi-original.yaml
authorization_urls: []
description: ''
docs: https://developers.hellosign.com/docs/guides/o-auth/walkthrough/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hellosign Scopes
name_suffix: OAuth Scopes
note: 'Dropbox Sign OAuth 2.0 scopes. The OpenAPI spec models the OAuth token only as an http bearer scheme (no flows/scope map), so scopes are captured here from the OAuth guide. Scopes are split by billing model: "app-owner charged" vs "user charged".'
overview: 'Dropbox Sign (HelloSign) publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dropbox Sign (HelloSign) API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dropbox Sign (HelloSign)
provider_slug: hellosign
schemes:
- authorizationUrl: https://app.hellosign.com/oauth/authorize
  flow: authorizationCode
  name: oauth2
  tokenUrl: https://app.hellosign.com/oauth/token
  type: oauth2
scope_count: 7
scope_names:
- basic_account_info
- request_signature
- account_access
- signature_request_access
- template_access
- team_access
- api_app_access
scopes:
- description: Access basic account information, such as email address and name.
  flows: []
  scope: basic_account_info
- description: Send signature requests, access statuses and document files.
  flows: []
  scope: request_signature
- description: Access to basic account information, such as email address and name.
  flows: []
  scope: account_access
- description: Access to send, view, and update signature requests and to download document files.
  flows: []
  scope: signature_request_access
- description: Access to view, create, and modify templates.
  flows: []
  scope: template_access
- description: Access to view and modify team settings and team members.
  flows: []
  scope: team_access
- description: Access to view, create, and modify embedded API apps.
  flows: []
  scope: api_app_access
slug: hellosign-scopes
source_filename: hellosign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.hellosign.com/docs/guides/o-auth/overview/\ndocs: https://developers.hellosign.com/docs/guides/o-auth/walkthrough/\nnote: >-\n  Dropbox Sign OAuth 2.0 scopes. The OpenAPI spec models the OAuth token only as\n  an http bearer scheme (no flows/scope map), so scopes are captured here from the\n  OAuth guide. Scopes are split by billing model: \"app-owner charged\" vs\n  \"user charged\".\nschemes:\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://app.hellosign.com/oauth/authorize\n    tokenUrl: https://app.hellosign.com/oauth/token\nscopes:\n  - scope: basic_account_info\n    billing: app-owner-charged\n    description: Access basic account information, such as email address and name.\n  - scope: request_signature\n    billing: app-owner-charged\n    description: Send signature requests, access statuses and document files.\n  - scope: account_access\n    billing:\
  \ user-charged\n    description: Access to basic account information, such as email address and name.\n  - scope: signature_request_access\n    billing: user-charged\n    description: Access to send, view, and update signature requests and to download document files.\n  - scope: template_access\n    billing: user-charged\n    description: Access to view, create, and modify templates.\n  - scope: team_access\n    billing: user-charged\n    description: Access to view and modify team settings and team members.\n  - scope: api_app_access\n    billing: user-charged\n    description: Access to view, create, and modify embedded API apps.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/scopes/hellosign-scopes.yml
summary_line: 7 scopes
tags:
- Company
- eSignature
- Electronic Signatures
- Documents
- Digital Agreements
- Signature Workflow
- Embedded Signing
- Compliance
token_urls: []
---
