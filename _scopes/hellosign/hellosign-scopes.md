---
api_specs:
- filename: hellosign-account-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Account API
  slug: hellosign-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-account-api-openapi.yml
- filename: hellosign-api-app-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Api App API
  slug: hellosign-api-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-api-app-api-openapi.yml
- filename: hellosign-bulk-send-job-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Bulk Send Job API
  slug: hellosign-bulk-send-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-bulk-send-job-api-openapi.yml
- filename: hellosign-embedded-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Embedded API
  slug: hellosign-embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-embedded-api-openapi.yml
- filename: hellosign-fax-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Fax API
  slug: hellosign-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-fax-api-openapi.yml
- filename: hellosign-fax-line-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Fax Line API
  slug: hellosign-fax-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-fax-line-api-openapi.yml
- filename: hellosign-oauth-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) OAuth API
  slug: hellosign-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-oauth-api-openapi.yml
- filename: hellosign-report-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Report API
  slug: hellosign-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-report-api-openapi.yml
- filename: hellosign-signature-request-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Signature Request API
  slug: hellosign-signature-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-signature-request-api-openapi.yml
- filename: hellosign-team-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Team API
  slug: hellosign-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-team-api-openapi.yml
- filename: hellosign-template-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Template API
  slug: hellosign-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-template-api-openapi.yml
- filename: hellosign-unclaimed-draft-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Unclaimed Draft API
  slug: hellosign-unclaimed-draft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-unclaimed-draft-api-openapi.yml
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
