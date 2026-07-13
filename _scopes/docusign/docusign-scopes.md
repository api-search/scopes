---
api_specs:
- filename: docusign-openapi-original.yml
  format: yaml
  label: Docusign eSignature REST API
  slug: docusign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-openapi-original.yml
- filename: docusign-admin-openapi-original.yml
  format: yaml
  label: Docusign Admin API
  slug: docusign-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-admin-openapi-original.yml
- filename: docusign-click-openapi-original.yml
  format: yaml
  label: Docusign Click API
  slug: docusign-click-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-click-openapi-original.yml
- filename: docusign-maestro-openapi-original.yml
  format: yaml
  label: Docusign Maestro API
  slug: docusign-maestro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-maestro-openapi-original.yml
- filename: docusign-monitor-openapi-original.yml
  format: yaml
  label: Docusign Monitor API
  slug: docusign-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-monitor-openapi-original.yml
- filename: docusign-rooms-openapi-original.yml
  format: yaml
  label: Docusign Rooms API
  slug: docusign-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-rooms-openapi-original.yml
authorization_urls:
- https://account.docusign.com/oauth/auth
- https://account-d.docusign.com/oauth/auth
- https://account-tk1.tk.docusign.dev/oauth/auth
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Docusign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Docusign publishes 13 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Docusign API on a user''s behalf.


  Tokens are issued from https://account.docusign.com/oauth/auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Docusign
provider_slug: docusign
schemes:
- description: OAuth2 Access code Grant
  flows:
  - authorizationUrl: https://account.docusign.com/oauth/auth
    flow: authorizationCode
    tokenUrl: https://account.docusign.com/oauth/auth
  name: accessCode
  source: openapi/docusign-admin-openapi-original.yml
- description: DocuSign uses OAuth 2.0. Supports Authorization Code Grant for user-present applications and JWT Grant for service integrations.
  flows:
  - authorizationUrl: https://account-d.docusign.com/oauth/auth
    flow: authorizationCode
    tokenUrl: https://account-d.docusign.com/oauth/token
  - authorizationUrl: https://account-d.docusign.com/oauth/auth
    flow: implicit
  name: OAuth2
  source: openapi/docusign-esignature-openapi.yml
- description: Docusign AuthN/AuthZ
  flows:
  - authorizationUrl: https://account-tk1.tk.docusign.dev/oauth/auth
    flow: authorizationCode
    tokenUrl: https://account-tk1.tk.docusign.dev/oauth/token
  name: DSAuth
  source: openapi/docusign-maestro-openapi-original.yml
scope_count: 13
scope_names:
- account_read
- account_write
- aow_manage
- domain_read
- extended
- group_read
- identity_provider_read
- impersonation
- organization_read
- permission_read
- signature
- user_read
- user_write
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: account_read
- description: ''
  flows:
  - authorizationCode
  scope: account_write
- description: Manage workflows scope
  flows:
  - authorizationCode
  scope: aow_manage
- description: ''
  flows:
  - authorizationCode
  scope: domain_read
- description: Extended API access
  flows:
  - authorizationCode
  scope: extended
- description: ''
  flows:
  - authorizationCode
  scope: group_read
- description: ''
  flows:
  - authorizationCode
  scope: identity_provider_read
- description: Impersonate users via JWT Grant
  flows:
  - authorizationCode
  scope: impersonation
- description: ''
  flows:
  - authorizationCode
  scope: organization_read
- description: ''
  flows:
  - authorizationCode
  scope: permission_read
- description: Access to signing and envelope operations
  flows:
  - authorizationCode
  - implicit
  scope: signature
- description: ''
  flows:
  - authorizationCode
  scope: user_read
- description: ''
  flows:
  - authorizationCode
  scope: user_write
slug: docusign-scopes
source_filename: docusign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docusign-admin-openapi-original.yml, openapi/docusign-esignature-openapi.yml,\n  openapi/docusign-maestro-openapi-original.yml\nschemes:\n- name: accessCode\n  source: openapi/docusign-admin-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.docusign.com/oauth/auth\n    tokenUrl: https://account.docusign.com/oauth/auth\n  description: OAuth2 Access code Grant\n- name: OAuth2\n  source: openapi/docusign-esignature-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account-d.docusign.com/oauth/auth\n    tokenUrl: https://account-d.docusign.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://account-d.docusign.com/oauth/auth\n  description: DocuSign uses OAuth 2.0. Supports Authorization Code Grant for user-present applications\n    and JWT Grant for service integrations.\n- name: DSAuth\n  source: openapi/docusign-maestro-openapi-original.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account-tk1.tk.docusign.dev/oauth/auth\n    tokenUrl: https://account-tk1.tk.docusign.dev/oauth/token\n  description: Docusign AuthN/AuthZ\nscopes:\n- scope: account_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: account_write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: aow_manage\n  description: Manage workflows scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-maestro-openapi-original.yml\n- scope: domain_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: extended\n  description: Extended API access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-esignature-openapi.yml\n- scope: group_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: identity_provider_read\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: impersonation\n  description: Impersonate users via JWT Grant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-esignature-openapi.yml\n- scope: organization_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: permission_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: signature\n  description: Access to signing and envelope operations\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/docusign-esignature-openapi.yml\n  - openapi/docusign-maestro-openapi-original.yml\n- scope: user_read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n- scope: user_write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docusign-admin-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/scopes/docusign-scopes.yml
summary_line: 13 scopes · authorizationCode/implicit
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
token_urls:
- https://account.docusign.com/oauth/auth
- https://account-d.docusign.com/oauth/token
- https://account-tk1.tk.docusign.dev/oauth/token
---
