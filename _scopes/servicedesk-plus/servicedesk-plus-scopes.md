---
api_specs:
- filename: servicedesk-plus-openapi.yml
  format: yaml
  label: ServiceDesk Plus REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/openapi/servicedesk-plus-openapi.yml
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Servicedesk Plus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ManageEngine ServiceDesk Plus publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ManageEngine ServiceDesk Plus API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ManageEngine ServiceDesk Plus
provider_slug: servicedesk-plus
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  source: openapi/servicedesk-plus-openapi.yml
scope_count: 5
scope_names:
- SDPOnDemand.requests.ALL
- SDPOnDemand.requests.CREATE
- SDPOnDemand.requests.DELETE
- SDPOnDemand.requests.READ
- SDPOnDemand.requests.UPDATE
scopes:
- description: Full access to requests
  flows:
  - authorizationCode
  scope: SDPOnDemand.requests.ALL
- description: Create requests
  flows:
  - authorizationCode
  scope: SDPOnDemand.requests.CREATE
- description: Delete requests
  flows:
  - authorizationCode
  scope: SDPOnDemand.requests.DELETE
- description: Read-only access to requests
  flows:
  - authorizationCode
  scope: SDPOnDemand.requests.READ
- description: Update requests
  flows:
  - authorizationCode
  scope: SDPOnDemand.requests.UPDATE
slug: servicedesk-plus-scopes
source_filename: servicedesk-plus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicedesk-plus-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/servicedesk-plus-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n- scope: SDPOnDemand.requests.ALL\n  description: Full access to requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n- scope: SDPOnDemand.requests.CREATE\n  description: Create requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n- scope: SDPOnDemand.requests.DELETE\n  description: Delete requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n- scope: SDPOnDemand.requests.READ\n  description: Read-only access to requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n- scope: SDPOnDemand.requests.UPDATE\n\
  \  description: Update requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicedesk-plus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/scopes/servicedesk-plus-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- ITSM
- Help Desk
- Incident Management
- Asset Management
- CMDB
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
