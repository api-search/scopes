---
authorization_urls:
- https://secure.adobesign.com/public/oauth/v2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Adobe Sign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Acrobat Sign publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Acrobat Sign API on a user''s behalf.


  Tokens are issued from https://secure.adobesign.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Acrobat Sign
provider_slug: adobe-sign
schemes:
- description: OAuth 2.0 authorization-code flow. The authorization code is exchanged at POST /oauth/v2/token for an access token (~3600s) and a refresh token. Scope modifiers :self, :group, and :account determine the authorization level.
  flows:
  - authorizationUrl: https://secure.adobesign.com/public/oauth/v2
    flow: authorizationCode
    tokenUrl: https://secure.adobesign.com/oauth/v2/token
  name: oauth2
  source: openapi/adobe-sign-openapi.yml
scope_count: 12
scope_names:
- agreement_read
- agreement_send
- agreement_write
- library_read
- library_write
- user_login
- user_read
- user_write
- widget_read
- widget_write
- workflow_read
- workflow_write
scopes:
- description: Read agreements
  flows:
  - authorizationCode
  scope: agreement_read
- description: Send agreements for signature
  flows:
  - authorizationCode
  scope: agreement_send
- description: Create and modify agreements
  flows:
  - authorizationCode
  scope: agreement_write
- description: Read library templates
  flows:
  - authorizationCode
  scope: library_read
- description: Create and modify library templates
  flows:
  - authorizationCode
  scope: library_write
- description: Sign in as a user
  flows:
  - authorizationCode
  scope: user_login
- description: Read user information
  flows:
  - authorizationCode
  scope: user_read
- description: Modify users
  flows:
  - authorizationCode
  scope: user_write
- description: Read widgets
  flows:
  - authorizationCode
  scope: widget_read
- description: Create and modify widgets
  flows:
  - authorizationCode
  scope: widget_write
- description: Read workflows
  flows:
  - authorizationCode
  scope: workflow_read
- description: Create and modify workflows
  flows:
  - authorizationCode
  scope: workflow_write
slug: adobe-sign-scopes
source_filename: adobe-sign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-sign-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/adobe-sign-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.adobesign.com/public/oauth/v2\n    tokenUrl: https://secure.adobesign.com/oauth/v2/token\n  description: OAuth 2.0 authorization-code flow. The authorization code is exchanged at POST\n    /oauth/v2/token for an access token (~3600s) and a refresh token. Scope modifiers :self,\n    :group, and :account determine the authorization level.\nscopes:\n- scope: agreement_read\n  description: Read agreements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: agreement_send\n  description: Send agreements for signature\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: agreement_write\n  description: Create and modify agreements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n\
  - scope: library_read\n  description: Read library templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: library_write\n  description: Create and modify library templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: user_login\n  description: Sign in as a user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: user_read\n  description: Read user information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: user_write\n  description: Modify users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: widget_read\n  description: Read widgets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: widget_write\n  description: Create and modify widgets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: workflow_read\n\
  \  description: Read workflows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n- scope: workflow_write\n  description: Create and modify workflows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-sign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-sign/refs/heads/main/scopes/adobe-sign-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Electronic Signature
- E-Signature
- Document Workflow
- Digital Signature
- Adobe
- Agreements
token_urls:
- https://secure.adobesign.com/oauth/v2/token
---
