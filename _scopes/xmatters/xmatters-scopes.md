---
api_specs:
- filename: xmatters-devices-api-openapi.yml
  format: yaml
  label: xMatters Devices API
  slug: xmatters-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-devices-api-openapi.yml
- filename: xmatters-events-api-openapi.yml
  format: yaml
  label: xMatters Events API
  slug: xmatters-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-events-api-openapi.yml
- filename: xmatters-groups-api-openapi.yml
  format: yaml
  label: xMatters Groups API
  slug: xmatters-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-groups-api-openapi.yml
- filename: xmatters-integrations-api-openapi.yml
  format: yaml
  label: xMatters Integrations API
  slug: xmatters-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-integrations-api-openapi.yml
- filename: xmatters-oncall-api-openapi.yml
  format: yaml
  label: xMatters OnCall API
  slug: xmatters-oncall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-oncall-api-openapi.yml
- filename: xmatters-people-api-openapi.yml
  format: yaml
  label: xMatters People API
  slug: xmatters-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-people-api-openapi.yml
- filename: xmatters-plans-api-openapi.yml
  format: yaml
  label: xMatters Plans API
  slug: xmatters-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-plans-api-openapi.yml
- filename: xmatters-scenarios-api-openapi.yml
  format: yaml
  label: xMatters Scenarios API
  slug: xmatters-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-scenarios-api-openapi.yml
- filename: xmatters-services-api-openapi.yml
  format: yaml
  label: xMatters Services API
  slug: xmatters-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-services-api-openapi.yml
- filename: xmatters-shifts-api-openapi.yml
  format: yaml
  label: xMatters Shifts API
  slug: xmatters-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-shifts-api-openapi.yml
authorization_urls: []
description: ''
docs: https://help.xmatters.com/ondemand/api/oauth.htm
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Xmatters Scopes
name_suffix: OAuth Scopes
note: xMatters OAuth 2.0 (password and refresh_token grants) does not use scopes; API access is governed by the authenticated user's roles and permissions (https://help.xmatters.com/xmapi/).
overview: 'xMatters uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: xMatters
provider_slug: xmatters
schemes:
- flows:
  - flow: password
    tokenUrl: https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token
  name: OAuth2
  source: openapi/xmatters-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: xmatters-scopes
source_filename: xmatters-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xmatters-openapi.yml\ndocs: https://help.xmatters.com/ondemand/api/oauth.htm\nnote: xMatters OAuth 2.0 (password and refresh_token grants) does not use scopes;\n  API access is governed by the authenticated user's roles and permissions\n  (https://help.xmatters.com/xmapi/).\nschemes:\n- name: OAuth2\n  source: openapi/xmatters-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/scopes/xmatters-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Incident Management
- On-Call
- Alerting
- Service Reliability
- DevOps
- Communication
- Workflow Automation
token_urls:
- https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token
---
