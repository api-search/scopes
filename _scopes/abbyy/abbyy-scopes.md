---
api_specs:
- filename: abbyy-catalogrecords-api-openapi.yml
  format: yaml
  label: ABBYY Catalog Records API
  slug: abbyy-catalogrecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-catalogrecords-api-openapi.yml
- filename: abbyy-catalogs-api-openapi.yml
  format: yaml
  label: ABBYY Catalogs API
  slug: abbyy-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-catalogs-api-openapi.yml
- filename: abbyy-invites-api-openapi.yml
  format: yaml
  label: ABBYY Invites API
  slug: abbyy-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-invites-api-openapi.yml
- filename: abbyy-report-api-openapi.yml
  format: yaml
  label: ABBYY Report API
  slug: abbyy-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-report-api-openapi.yml
- filename: abbyy-report-v1-api-openapi.yml
  format: yaml
  label: ABBYY Report v1 API
  slug: abbyy-report-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-report-v1-api-openapi.yml
- filename: abbyy-skills-api-openapi.yml
  format: yaml
  label: ABBYY Skills API
  slug: abbyy-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-skills-api-openapi.yml
- filename: abbyy-transactions-api-openapi.yml
  format: yaml
  label: ABBYY Transactions API
  slug: abbyy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-transactions-api-openapi.yml
- filename: abbyy-transaction-documents-api-openapi.yml
  format: yaml
  label: ABBYY Transaction Documents API
  slug: abbyy-transaction-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-transaction-documents-api-openapi.yml
authorization_urls:
- https://vantage-us.abbyy.com/auth2/connect/authorize
description: ''
docs: https://docs.abbyy.com/vantage/developer/authentication/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Abbyy Scopes
name_suffix: OAuth Scopes
note: 'ABBYY publishes exactly three OAuth scopes and no per-resource scope taxonomy: authorization is enforced by Vantage tenant ROLES (Tenant Administrator, Processing Supervisor, and so on) rather than by scope. global.wildcard grants the whole API surface — there is no read-only or per-resource scope a client can request instead, which is a real least-privilege gap for agent integrations. No scopes/permissions reference page exists in the public docs; searched 2026-08-29 and none found.'
overview: 'ABBYY publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ABBYY API on a user''s behalf.


  Tokens are issued from https://vantage-us.abbyy.com/auth2/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ABBYY
provider_slug: abbyy
schemes:
- flows:
  - authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize
    flow: authorizationCode
    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token
  name: OAuth2Security
  source: openapi/abbyy-vantage-processing-openapi.yml
- flows:
  - authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize
    flow: authorizationCode
    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token
  name: OAuth2Security
  source: openapi/abbyy-vantage-reporting-openapi.yml
- flows:
  - authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize
    flow: authorizationCode
    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token
  name: OAuth2Security
  source: openapi/abbyy-vantage-reporting-v1-openapi.yml
scope_count: 3
scope_names:
- global.wildcard
- openid
- permissions
scopes:
- description: Global wildcard
  flows:
  - authorizationCode
  scope: global.wildcard
- description: User Id
  flows:
  - authorizationCode
  scope: openid
- description: User permissions
  flows:
  - authorizationCode
  scope: permissions
slug: abbyy-scopes
source_filename: abbyy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/_original/abbyy-vantage-processing-openapi.json (https://docs.abbyy.com/openapi.json, HTTP 200)\n  plus the ABBYY Vantage authentication docs\nschemes:\n- name: OAuth2Security\n  source: openapi/abbyy-vantage-processing-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize\n    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token\n- name: OAuth2Security\n  source: openapi/abbyy-vantage-reporting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize\n    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token\n- name: OAuth2Security\n  source: openapi/abbyy-vantage-reporting-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vantage-us.abbyy.com/auth2/connect/authorize\n    tokenUrl: https://vantage-us.abbyy.com/auth2/connect/token\n\
  scopes:\n- scope: global.wildcard\n  description: Global wildcard\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/abbyy-vantage-processing-openapi.yml\n  - openapi/abbyy-vantage-reporting-openapi.yml\n  - openapi/abbyy-vantage-reporting-v1-openapi.yml\n- scope: openid\n  description: User Id\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/abbyy-vantage-processing-openapi.yml\n  - openapi/abbyy-vantage-reporting-openapi.yml\n  - openapi/abbyy-vantage-reporting-v1-openapi.yml\n- scope: permissions\n  description: User permissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/abbyy-vantage-processing-openapi.yml\n  - openapi/abbyy-vantage-reporting-openapi.yml\n  - openapi/abbyy-vantage-reporting-v1-openapi.yml\ndocs: https://docs.abbyy.com/vantage/developer/authentication/authentication\nnote: 'ABBYY publishes exactly three OAuth scopes and no per-resource scope taxonomy: authorization is enforced\n  by Vantage tenant ROLES (Tenant Administrator, Processing\
  \ Supervisor, and so on) rather than by scope. global.wildcard\n  grants the whole API surface — there is no read-only or per-resource scope a client can request instead, which\n  is a real least-privilege gap for agent integrations. No scopes/permissions reference page exists in the public\n  docs; searched 2026-08-29 and none found.'\nrole_based_restrictions:\n- api: ABBYY Vantage Reporting API\n  restriction: Tenant Administrator or Processing Supervisor role required to download data reports\n  evidence: info.description of openapi-reporting.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/scopes/abbyy-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- AI Automation
- Document Processing
- OCR
- Intelligent Document Processing
- Data Extraction
- Process Intelligence
- MCP
- Agent Skills
- RPA
- Enterprise Automation
- A2A
token_urls:
- https://vantage-us.abbyy.com/auth2/connect/token
---
