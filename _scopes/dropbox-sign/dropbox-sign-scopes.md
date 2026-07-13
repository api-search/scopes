---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Dropbox Sign REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/hellosign/hellosign-openapi/blob/main/openapi.yaml
- filename: dropbox-sign-events-asyncapi.yml
  format: yaml
  label: Dropbox Sign Events and Callbacks API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/asyncapi/dropbox-sign-events-asyncapi.yml
authorization_urls:
- https://app.hellosign.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Dropbox Sign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dropbox Sign publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dropbox Sign API on a user''s behalf.


  Tokens are issued from https://app.hellosign.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dropbox Sign
provider_slug: dropbox-sign
schemes:
- flows:
  - authorizationUrl: https://app.hellosign.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.hellosign.com/oauth/token
  name: oauth2
  source: openapi/dropbox-sign-openapi.yml
scope_count: 5
scope_names:
- account_access
- api_app_access
- basic_account_info
- signature_request_access
- template_access
scopes:
- description: Manage account
  flows:
  - authorizationCode
  scope: account_access
- description: Manage API apps
  flows:
  - authorizationCode
  scope: api_app_access
- description: View basic account info
  flows:
  - authorizationCode
  scope: basic_account_info
- description: Manage signature requests
  flows:
  - authorizationCode
  scope: signature_request_access
- description: Manage templates
  flows:
  - authorizationCode
  scope: template_access
slug: dropbox-sign-scopes
source_filename: dropbox-sign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dropbox-sign-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/dropbox-sign-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hellosign.com/oauth/authorize\n    tokenUrl: https://app.hellosign.com/oauth/token\nscopes:\n- scope: account_access\n  description: Manage account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n- scope: api_app_access\n  description: Manage API apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n- scope: basic_account_info\n  description: View basic account info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n- scope: signature_request_access\n  description: Manage signature requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dropbox-sign-openapi.yml\n- scope: template_access\n  description: Manage templates\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/dropbox-sign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/scopes/dropbox-sign-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- eSignature
- Electronic Signature
- Document Signing
- Workflow Automation
- Documents
token_urls:
- https://app.hellosign.com/oauth/token
---
