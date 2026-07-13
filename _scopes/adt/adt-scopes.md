---
api_specs:
- filename: adt-platform-api-openapi.yml
  format: yaml
  label: ADT+ Platform API
  slug: adt-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-platform-api-openapi.yml
- filename: adt-business-api-openapi.yml
  format: yaml
  label: ADT Business API
  slug: adt-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-business-api-openapi.yml
authorization_urls:
- https://auth.adt.com/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Adt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ADT publishes 10 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ADT API on a user''s behalf.


  Tokens are issued from https://auth.adt.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ADT
provider_slug: adt
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.adt.com/oauth/token
  name: oauth2
  source: openapi/adt-business-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.adt.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.adt.com/oauth/token
  name: oauth2
  source: openapi/adt-platform-api-openapi.yml
scope_count: 10
scope_names:
- access-codes:manage
- access-control:manage
- business:read
- business:write
- devices:read
- devices:write
- reports:read
- security:read
- security:write
- video:read
scopes:
- description: Manage access codes
  flows:
  - authorizationCode
  scope: access-codes:manage
- description: Manage access control
  flows:
  - clientCredentials
  scope: access-control:manage
- description: Read business site data
  flows:
  - clientCredentials
  scope: business:read
- description: Manage business security systems
  flows:
  - clientCredentials
  scope: business:write
- description: Read device status
  flows:
  - authorizationCode
  scope: devices:read
- description: Control smart home devices
  flows:
  - authorizationCode
  scope: devices:write
- description: Generate security reports
  flows:
  - clientCredentials
  scope: reports:read
- description: Read security system status and events
  flows:
  - authorizationCode
  scope: security:read
- description: Arm, disarm, and control security systems
  flows:
  - authorizationCode
  scope: security:write
- description: Access video clips and live streams
  flows:
  - authorizationCode
  scope: video:read
slug: adt-scopes
source_filename: adt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adt-business-api-openapi.yml, openapi/adt-platform-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/adt-business-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.adt.com/oauth/token\n- name: oauth2\n  source: openapi/adt-platform-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.adt.com/oauth/authorize\n    tokenUrl: https://auth.adt.com/oauth/token\nscopes:\n- scope: access-codes:manage\n  description: Manage access codes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n- scope: access-control:manage\n  description: Manage access control\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adt-business-api-openapi.yml\n- scope: business:read\n  description: Read business site data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adt-business-api-openapi.yml\n- scope: business:write\n\
  \  description: Manage business security systems\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adt-business-api-openapi.yml\n- scope: devices:read\n  description: Read device status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n- scope: devices:write\n  description: Control smart home devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n- scope: reports:read\n  description: Generate security reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adt-business-api-openapi.yml\n- scope: security:read\n  description: Read security system status and events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n- scope: security:write\n  description: Arm, disarm, and control security systems\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n- scope: video:read\n  description: Access video clips and live streams\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/scopes/adt-scopes.yml
summary_line: 10 scopes · clientCredentials/authorizationCode
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
token_urls:
- https://auth.adt.com/oauth/token
---
