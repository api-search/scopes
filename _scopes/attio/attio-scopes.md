---
api_specs:
- filename: openapi
  format: yaml
  label: Attio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.attio.com/rest-api/endpoint-reference/openapi
authorization_urls:
- https://app.attio.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Attio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Attio publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Attio API on a user''s behalf.


  Tokens are issued from https://api.attio.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Attio
provider_slug: attio
schemes:
- flows:
  - authorizationUrl: https://app.attio.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.attio.com/oauth/token
  name: oauth2
  source: openapi/attio-openapi.yml
scope_count: 7
scope_names:
- list_configuration:read-write
- list_entry:read-write
- object_configuration:read
- object_configuration:read-write
- record_permission:read
- record_permission:read-write
- webhook:read-write
scopes:
- description: Manage lists
  flows:
  - authorizationCode
  scope: list_configuration:read-write
- description: Manage list entries
  flows:
  - authorizationCode
  scope: list_entry:read-write
- description: Read object configuration
  flows:
  - authorizationCode
  scope: object_configuration:read
- description: Manage object configuration
  flows:
  - authorizationCode
  scope: object_configuration:read-write
- description: Read records
  flows:
  - authorizationCode
  scope: record_permission:read
- description: Manage records
  flows:
  - authorizationCode
  scope: record_permission:read-write
- description: Manage webhooks
  flows:
  - authorizationCode
  scope: webhook:read-write
slug: attio-scopes
source_filename: attio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attio-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/attio-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.attio.com/authorize\n    tokenUrl: https://api.attio.com/oauth/token\nscopes:\n- scope: list_configuration:read-write\n  description: Manage lists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n- scope: list_entry:read-write\n  description: Manage list entries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n- scope: object_configuration:read\n  description: Read object configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n- scope: object_configuration:read-write\n  description: Manage object configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n- scope: record_permission:read\n  description: Read records\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/attio-openapi.yml\n- scope: record_permission:read-write\n  description: Manage records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n- scope: webhook:read-write\n  description: Manage webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/scopes/attio-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- CRM
- Customer Relationship Management
- Sales
- Contacts
- Companies
- Pipeline
- Workflows
token_urls:
- https://api.attio.com/oauth/token
---
