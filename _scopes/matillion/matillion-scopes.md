---
api_specs:
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Projects
  slug: dpc-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Environments
  slug: dpc-environments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Pipeline Executions
  slug: dpc-pipeline-executions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Schedules
  slug: dpc-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Agents
  slug: dpc-agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Groups & Projects (legacy)
  slug: etl-groups-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Jobs & Runs (legacy)
  slug: etl-jobs-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Tasks (legacy)
  slug: etl-tasks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Schedules (legacy)
  slug: etl-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.maia.ai/docs/api-reference/maia-api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Matillion Scopes
name_suffix: OAuth Scopes
note: Matillion does not publish a scopes catalog; API access is permissioned via roles on API credentials (account, project, and environment roles), and the token response's scope is fixed at pipeline-execution (https://docs.maia.ai/docs/api-reference/maia-api-authentication).
overview: 'Matillion publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Matillion API on a user''s behalf.


  Tokens are issued from https://id.core.matillion.com/oauth/dpc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Matillion
provider_slug: matillion
schemes:
- description: 'Data Productivity Cloud OAuth2 client-credentials flow. Exchange your client id and secret for a Bearer JWT at the token URL, requesting the audience https://api.matillion.com, then send it as Authorization: Bearer <JWT>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://id.core.matillion.com/oauth/dpc/token
  name: dpc_oauth
  source: openapi/matillion-openapi.yml
scope_count: 1
scope_names:
- pipeline-execution
scopes:
- description: The only scope value documented for the Data Productivity Cloud (Maia) API; it appears in the client-credentials token response. Callers do not request scopes - effective permissions are governed by the account role assigned to the API credential set, plus project and environment roles for non-Super Admin credentials.
  flows: []
  scope: pipeline-execution
slug: matillion-scopes
source_filename: matillion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/matillion-openapi.yml\ndocs: https://docs.maia.ai/docs/api-reference/maia-api-authentication\nschemes:\n- name: dpc_oauth\n  source: openapi/matillion-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.core.matillion.com/oauth/dpc/token\n  description: 'Data Productivity Cloud OAuth2 client-credentials flow. Exchange your client\n    id and secret for a Bearer JWT at the token URL, requesting the audience https://api.matillion.com,\n    then send it as Authorization: Bearer <JWT>.'\nscopes:\n- scope: pipeline-execution\n  description: The only scope value documented for the Data Productivity Cloud (Maia)\n    API; it appears in the client-credentials token response. Callers do not request\n    scopes - effective permissions are governed by the account role assigned to the\n    API credential set, plus project and environment roles for non-Super Admin credentials.\n  sources:\n  - https://docs.maia.ai/docs/api-reference/maia-api-authentication\n\
  note: Matillion does not publish a scopes catalog; API access is permissioned via\n  roles on API credentials (account, project, and environment roles), and the token\n  response's scope is fixed at pipeline-execution (https://docs.maia.ai/docs/api-reference/maia-api-authentication).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/scopes/matillion-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Data Integration
- ETL
- ELT
- Data Pipelines
- Cloud Data Warehouse
token_urls:
- https://id.core.matillion.com/oauth/dpc/token
---
