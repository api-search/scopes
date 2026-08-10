---
api_specs:
- filename: element-biosciences-authservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Auth Service API
  slug: element-biosciences-authservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-authservice-api-openapi.yml
- filename: element-biosciences-executionservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Execution Service API
  slug: element-biosciences-executionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-executionservice-api-openapi.yml
- filename: element-biosciences-instrumentservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Instrument Service API
  slug: element-biosciences-instrumentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-instrumentservice-api-openapi.yml
- filename: element-biosciences-runservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Run Service API
  slug: element-biosciences-runservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-runservice-api-openapi.yml
- filename: element-biosciences-storageconnectionservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Storage Connection Service API
  slug: element-biosciences-storageconnectionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-storageconnectionservice-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.elembio.io/docs/elembio-cloud/api-keys/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Element Biosciences Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Element Biosciences publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Element Biosciences API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Element Biosciences
provider_slug: element-biosciences
schemes: []
scope_count: 12
scope_names:
- Runs
- Runs:Read
- Runs:Download
- Executions
- Executions:Read
- Executions:Download
- Executions:Logs
- Instruments
- Instruments:Read
- Storage
- Storage:Read
- Storage:Download
scopes:
- description: Unrestricted access to all run data, including read, download, edit, and all other actions.
  flows: []
  scope: Runs
- description: List and get run metadata for all runs.
  flows: []
  scope: Runs:Read
- description: Browse and download run files for all runs.
  flows: []
  scope: Runs:Download
- description: Unrestricted access to all analysis executions, including read, download, edit, and all other actions.
  flows: []
  scope: Executions
- description: List and get executions metadata for all executions.
  flows: []
  scope: Executions:Read
- description: Browse and download executions files for all executions.
  flows: []
  scope: Executions:Download
- description: View logs for all executions.
  flows: []
  scope: Executions:Logs
- description: Unrestricted access to all instrument metadata.
  flows: []
  scope: Instruments
- description: List and get instrument metadata for all instruments.
  flows: []
  scope: Instruments:Read
- description: Unrestricted access to all storage connections and data.
  flows: []
  scope: Storage
- description: List and get storage metadata for all storage connections.
  flows: []
  scope: Storage:Read
- description: Browse and download storage files for all storage connections. Narrowable to a specific connection or path prefix.
  flows: []
  scope: Storage:Download
slug: element-biosciences-scopes
source_filename: element-biosciences-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.elembio.io/docs/elembio-cloud/api-keys/\ndocs: https://docs.elembio.io/docs/elembio-cloud/api-keys/\noauth2: false\nscheme_type: apiKey\nscheme_note: |\n  IMPORTANT — these are NOT OAuth 2.0 scopes. The Element Biosciences Cloud API\n  authenticates with a static API key in the x-api-key header; there is no OAuth\n  authorization server, no token endpoint and no consent flow. Each API key is\n  nonetheless issued with an explicit permission set, and the OpenAPI describes the\n  grammar as `resource:action[:resource_id]`. This artifact captures that real,\n  documented permission model. It is filed under scopes/ because it is the provider's\n  scope surface, and the apis.yml pointer uses the catalog's canonical scope type.\ngrammar: 'resource:action[:resource_id]'\ngrammar_source: openapi/element-biosciences-cloud-api-openapi-original.yml (info.description)\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_reason:\
  \ INSUFFICIENT_SCOPE\n  list_behaviour: List endpoints transparently restrict results to the resources a key is scoped to.\nkey_policy:\n  expiration_days: {min: 1, max: 365, default: 30}\n  revocation: Deleting a key immediately revokes it; the action cannot be undone.\n  name_max_length: 256\n  description_max_length: 500\n  creation_path: Organization > API Keys > Add API Key\n  guidance: Grant the minimum required permissions (principle of least privilege); never commit keys to source control.\nscopes:\n- scope: Runs\n  api_form: 'runs:*'\n  description: Unrestricted access to all run data, including read, download, edit, and all other actions.\n  group: Runs\n- scope: Runs:Read\n  api_form: 'runs:read'\n  description: List and get run metadata for all runs.\n  group: Runs\n  operations: [RunService_ListRuns, RunService_GetRun]\n- scope: Runs:Download\n  api_form: 'runs:download'\n  description: Browse and download run files for all runs.\n  group: Runs\n  operations: [RunService_ListRunFiles,\
  \ RunService_GetRunDownloadCredentials]\n- scope: Executions\n  api_form: 'executions:*'\n  description: Unrestricted access to all analysis executions, including read, download, edit, and all other actions.\n  group: Executions\n- scope: Executions:Read\n  api_form: 'executions:read'\n  description: List and get executions metadata for all executions.\n  group: Executions\n  operations: [ExecutionService_ListExecutions, ExecutionService_GetExecution]\n- scope: Executions:Download\n  api_form: 'executions:download'\n  description: Browse and download executions files for all executions.\n  group: Executions\n  operations: [ExecutionService_ListExecutionFiles, ExecutionService_GetExecutionDownloadCredentials]\n- scope: Executions:Logs\n  api_form: 'executions:logs'\n  description: View logs for all executions.\n  group: Executions\n  operations: [ExecutionService_GetExecutionLogs]\n- scope: Instruments\n  api_form: 'instruments:*'\n  description: Unrestricted access to all instrument metadata.\n\
  \  group: Instruments\n- scope: Instruments:Read\n  api_form: 'instruments:read'\n  description: List and get instrument metadata for all instruments.\n  group: Instruments\n  operations: [InstrumentService_ListInstruments, InstrumentService_GetInstrument]\n- scope: Storage\n  api_form: 'storage:*'\n  description: Unrestricted access to all storage connections and data.\n  group: Storage\n- scope: Storage:Read\n  api_form: 'storage:read'\n  description: List and get storage metadata for all storage connections.\n  group: Storage\n  operations: [StorageConnectionService_ListStorageConnections, StorageConnectionService_GetStorageConnection]\n- scope: Storage:Download\n  api_form: 'storage:download[:connection_id]'\n  description: Browse and download storage files for all storage connections. Narrowable to a specific connection or path prefix.\n  group: Storage\n  operations: [StorageConnectionService_ListFiles, StorageConnectionService_GetDownloadCredentials]\n  resource_scopable: true\n\
  introspection:\n  operation: AuthService_GetAuth\n  path: GET /v1/auth\n  returns: [tenantId, scopes]\n  note: Call GET /v1/auth to confirm which tenant a key belongs to and which scopes it carries.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/scopes/element-biosciences-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Genomics
- DNA Sequencing
- Life Sciences
- Bioinformatics
- Multiomics
- Laboratory
- Scientific Instruments
- Cloud Storage
- Biotechnology
token_urls: []
---
