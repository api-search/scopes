---
api_specs:
- filename: power-query-fabric-dataflow-swagger.json
  format: json
  label: Fabric Dataflow REST API (Power Query)
  slug: fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-query/refs/heads/main/openapi/power-query-fabric-dataflow-swagger.json
authorization_urls: []
description: 'Microsoft Entra ID delegated scopes governing the Power Query (Fabric Dataflow) REST surface. Fabric draws a generic/specific distinction: generic `Item.*` scopes grant a token over any item type, specific `Dataflow.*` scopes narrow it to dataflows. Scopes apply ONLY to delegated, on-behalf-of-user access; service principals and managed identities are governed by Fabric admin controls and workspace permissions instead. The scopes are not declared in the published Swagger — they are carried in each operation''s `Required Delegated Scopes` prose section, which is where the list below was read from.'
docs: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Power Query Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Power Query uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Power Query
provider_slug: power-query
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: power-query-scopes
source_filename: power-query-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes\ndocs: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes\nprovider: Power Query\nproviderId: power-query\ndescription: >-\n  Microsoft Entra ID delegated scopes governing the Power Query (Fabric Dataflow)\n  REST surface. Fabric draws a generic/specific distinction: generic `Item.*`\n  scopes grant a token over any item type, specific `Dataflow.*` scopes narrow it\n  to dataflows. Scopes apply ONLY to delegated, on-behalf-of-user access; service\n  principals and managed identities are governed by Fabric admin controls and\n  workspace permissions instead. The scopes are not declared in the published\n  Swagger — they are carried in each operation's `Required Delegated Scopes`\n  prose section, which is where the list below was read from.\nflow: authorization_code\nauthorization_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n\
  token_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/token\noidc_scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\nscopes:\n  - name: Dataflow.Read.All\n    kind: specific\n    description: Read all dataflows the signed-in user has access to.\n    verified_on:\n      - Items_GetDataflow\n      - Items_DiscoverDataflowParameters\n  - name: Dataflow.ReadWrite.All\n    kind: specific\n    description: Read and write all dataflows the signed-in user has access to.\n    verified_on:\n      - Items_CreateDataflow\n      - Items_UpdateDataflow\n      - Items_DeleteDataflow\n      - Items_GetDataflowDefinition\n      - Items_UpdateDataflowDefinition\n      - BackgroundJobs_ScheduleExecute\n      - BackgroundJobs_ScheduleApplyChanges\n  - name: Dataflow.Execute.All\n    kind: specific\n    description: Execute dataflows the signed-in user has access to.\n    verified_on:\n      - QueryExecution_ExecuteQuery\n      - BackgroundJobs_ScheduleExecute\n      - BackgroundJobs_ScheduleApplyChanges\n\
  \    note: >-\n      The two schedule operations require Dataflow.Execute.All AND\n      Dataflow.ReadWrite.All together, not either/or.\n  - name: Dataflow.Reshare.All\n    kind: specific\n    description: >-\n      Reshare dataflows the signed-in user has access to. Documented by the\n      Fabric scopes article as part of the <itemType>.Reshare.All pattern; no\n      Dataflow operation in the published spec was observed requiring it.\n    verified_on: []\n  - name: Workspace.Read.All\n    kind: other\n    description: Read the workspaces the signed-in user has access to.\n    verified_on:\n      - Items_ListDataflows\n  - name: Workspace.ReadWrite.All\n    kind: other\n    description: Read and write the workspaces the signed-in user has access to.\n    verified_on:\n      - Items_ListDataflows\n  - name: Item.Read.All\n    kind: generic\n    description: Read all Fabric items of any type the signed-in user has access to.\n    verified_on:\n      - Items_GetDataflow\n      - Items_DiscoverDataflowParameters\n\
  \  - name: Item.ReadWrite.All\n    kind: generic\n    description: Read and write all Fabric items of any type.\n    verified_on:\n      - Items_CreateDataflow\n      - Items_UpdateDataflow\n      - Items_DeleteDataflow\n      - Items_GetDataflowDefinition\n      - Items_UpdateDataflowDefinition\n      - Items_GetDataflow\n  - name: Item.Execute.All\n    kind: generic\n    description: Execute all Fabric items.\n    verified_on:\n      - QueryExecution_ExecuteQuery\n  - name: Item.Reshare.All\n    kind: generic\n    description: Reshare all Fabric items.\n    verified_on: []\nunverified_operations:\n  - operation: BackgroundJobs_RunOnDemandExecute\n    reason: >-\n      No reference page was located under\n      /rest/api/fabric/dataflow/background-jobs/ for this operation on 2026-08-29,\n      so its Required Delegated Scopes block could not be read. Not inferred.\n  - operation: BackgroundJobs_RunOnDemandApplyChanges\n    reason: Same as above.\nnotes:\n  - >-\n    Every operation additionally\
  \ requires a Fabric workspace role. A token\n    carrying Dataflow.ReadWrite.All does not by itself permit creating a dataflow\n    — the caller must also hold the contributor workspace role.\n  - >-\n    The full delegated-scope catalog is enumerated in the Azure portal under\n    App registrations > Add permissions > Power BI Service.\nevidence:\n  - url: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes\n    status: 200\n  - url: https://learn.microsoft.com/en-us/rest/api/fabric/dataflow/items/create-dataflow\n    status: 200\n  - url: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n    status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n    url: https://apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-query/refs/heads/main/scopes/power-query-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Business Intelligence
- Data Integration
- Data Transformation
- ETL
- Microsoft
- Microsoft Fabric
- Power BI
- Dataflows
- M Language
- Data Connectors
- Self-Service ETL
token_urls: []
---
