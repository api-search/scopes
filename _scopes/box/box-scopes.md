---
authorization_urls:
- https://account.box.com/api/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Box Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Box publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Box API on a user''s behalf.


  Tokens are issued from https://api.box.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Box
provider_slug: box
schemes:
- flows:
  - authorizationUrl: https://account.box.com/api/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.box.com/oauth2/token
  name: OAuth2Security
  source: openapi/box-openapi-original.yml
scope_count: 9
scope_names:
- manage_app_users
- manage_data_retention
- manage_enterprise_properties
- manage_groups
- manage_legal_hold
- manage_managed_users
- manage_webhook
- root_readonly
- root_readwrite
scopes:
- description: Provision and manage app users
  flows:
  - authorizationCode
  scope: manage_app_users
- description: Manage data retention polices
  flows:
  - authorizationCode
  scope: manage_data_retention
- description: Manage enterprise properties
  flows:
  - authorizationCode
  scope: manage_enterprise_properties
- description: Manage an enterprise's groups
  flows:
  - authorizationCode
  scope: manage_groups
- description: Manage Legal Holds
  flows:
  - authorizationCode
  scope: manage_legal_hold
- description: Provision and manage managed users
  flows:
  - authorizationCode
  scope: manage_managed_users
- description: Create webhooks programmatically through the API
  flows:
  - authorizationCode
  scope: manage_webhook
- description: Read all files and folders stored in Box
  flows:
  - authorizationCode
  scope: root_readonly
- description: Read and write all files and folders stored in Box
  flows:
  - authorizationCode
  scope: root_readwrite
slug: box-scopes
source_filename: box-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/box-openapi-original.yml\nschemes:\n- name: OAuth2Security\n  source: openapi/box-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.box.com/api/oauth2/authorize\n    tokenUrl: https://api.box.com/oauth2/token\nscopes:\n- scope: manage_app_users\n  description: Provision and manage app users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_data_retention\n  description: Manage data retention polices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_enterprise_properties\n  description: Manage enterprise properties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_groups\n  description: Manage an enterprise's groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_legal_hold\n\
  \  description: Manage Legal Holds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_managed_users\n  description: Provision and manage managed users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: manage_webhook\n  description: Create webhooks programmatically through the API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: root_readonly\n  description: Read all files and folders stored in Box\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n- scope: root_readwrite\n  description: Read and write all files and folders stored in Box\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/box-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/box/refs/heads/main/scopes/box-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Cloud Storage
- Collaboration
- Content Management
- Documents
- Enterprise
- File Sharing
token_urls:
- https://api.box.com/oauth2/token
---
