---
api_specs:
- filename: egnyte-openapi.yml
  format: yaml
  label: Egnyte Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egnyte/refs/heads/main/openapi/egnyte-openapi.yml
authorization_urls:
- https://{domain}.egnyte.com/puboauth/token
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Egnyte Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Egnyte publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Egnyte API on a user''s behalf.


  Tokens are issued from https://{domain}.egnyte.com/puboauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Egnyte
provider_slug: egnyte
schemes:
- flows:
  - authorizationUrl: https://{domain}.egnyte.com/puboauth/token
    flow: authorizationCode
    tokenUrl: https://{domain}.egnyte.com/puboauth/token
  name: oauth2
  source: openapi/egnyte-openapi.yml
scope_count: 6
scope_names:
- Egnyte.audit
- Egnyte.filesystem
- Egnyte.group
- Egnyte.link
- Egnyte.permission
- Egnyte.user
scopes:
- description: Audit report access
  flows:
  - authorizationCode
  scope: Egnyte.audit
- description: File system access
  flows:
  - authorizationCode
  scope: Egnyte.filesystem
- description: Group management
  flows:
  - authorizationCode
  scope: Egnyte.group
- description: Shared link management
  flows:
  - authorizationCode
  scope: Egnyte.link
- description: Permission management
  flows:
  - authorizationCode
  scope: Egnyte.permission
- description: User management
  flows:
  - authorizationCode
  scope: Egnyte.user
slug: egnyte-scopes
source_filename: egnyte-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/egnyte-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/egnyte-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{domain}.egnyte.com/puboauth/token\n    tokenUrl: https://{domain}.egnyte.com/puboauth/token\nscopes:\n- scope: Egnyte.audit\n  description: Audit report access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n- scope: Egnyte.filesystem\n  description: File system access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n- scope: Egnyte.group\n  description: Group management\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n- scope: Egnyte.link\n  description: Shared link management\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n- scope: Egnyte.permission\n  description: Permission management\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n\
  - scope: Egnyte.user\n  description: User management\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/egnyte-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/egnyte/refs/heads/main/scopes/egnyte-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- File Sharing
- Content Collaboration
- Enterprise Storage
- Document Management
- Governance
- Data Security
token_urls:
- https://{domain}.egnyte.com/puboauth/token
---
