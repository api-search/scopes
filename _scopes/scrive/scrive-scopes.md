---
api_specs:
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Documents API
  slug: scrive-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Templates API
  slug: scrive-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Signing API
  slug: scrive-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive e-ID Authentication API
  slug: scrive-eid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Attachments API
  slug: scrive-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Callbacks API
  slug: scrive-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Access Control API
  slug: scrive-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
authorization_urls:
- https://oauth2.scrive.com/oauth2/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Scrive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Scrive publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Scrive API on a user''s behalf.


  Tokens are issued from https://oauth2.scrive.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scrive
provider_slug: scrive
schemes:
- flows:
  - authorizationUrl: https://oauth2.scrive.com/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://oauth2.scrive.com/oauth2/token
  name: oauth2
  source: openapi/scrive-openapi.yml
scope_count: 6
scope_names:
- doc:check
- doc:create
- doc:send
- full
- offline_access
- openid
scopes:
- description: Read documents
  flows:
  - authorizationCode
  scope: doc:check
- description: Create documents
  flows:
  - authorizationCode
  scope: doc:create
- description: Send documents
  flows:
  - authorizationCode
  scope: doc:send
- description: Full access
  flows:
  - authorizationCode
  scope: full
- description: Refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
slug: scrive-scopes
source_filename: scrive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrive-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/scrive-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.scrive.com/oauth2/authorization\n    tokenUrl: https://oauth2.scrive.com/oauth2/token\nscopes:\n- scope: doc:check\n  description: Read documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n- scope: doc:create\n  description: Create documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n- scope: doc:send\n  description: Send documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n- scope: full\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n- scope: offline_access\n  description: Refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n- scope: openid\n  description: OpenID\
  \ Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/scrive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/scopes/scrive-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- E-Signature
- Electronic Signing
- Digital Identity
- e-ID
- BankID
- MitID
- Nordic
- Document Workflow
token_urls:
- https://oauth2.scrive.com/oauth2/token
---
