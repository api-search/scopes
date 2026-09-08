---
api_specs:
- filename: n8n-public-api-openapi.yml
  format: yaml
  label: N8n
  slug: n8n
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-public-api-openapi.yml
- filename: n8n-audit-api-openapi.yml
  format: yaml
  label: N8n Audit API
  slug: n8n-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-audit-api-openapi.yml
- filename: n8n-communitypackage-api-openapi.yml
  format: yaml
  label: N8n CommunityPackage API
  slug: n8n-communitypackage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-communitypackage-api-openapi.yml
- filename: n8n-credential-api-openapi.yml
  format: yaml
  label: N8n Credential API
  slug: n8n-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-credential-api-openapi.yml
- filename: n8n-datatable-api-openapi.yml
  format: yaml
  label: N8n DataTable API
  slug: n8n-datatable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-datatable-api-openapi.yml
- filename: n8n-discover-api-openapi.yml
  format: yaml
  label: N8n Discover API
  slug: n8n-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-discover-api-openapi.yml
- filename: n8n-execution-api-openapi.yml
  format: yaml
  label: N8n Execution API
  slug: n8n-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-execution-api-openapi.yml
- filename: n8n-folders-api-openapi.yml
  format: yaml
  label: N8n Folders API
  slug: n8n-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-folders-api-openapi.yml
- filename: n8n-insights-api-openapi.yml
  format: yaml
  label: N8n Insights API
  slug: n8n-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-insights-api-openapi.yml
- filename: n8n-projects-api-openapi.yml
  format: yaml
  label: N8n Projects API
  slug: n8n-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-projects-api-openapi.yml
- filename: n8n-sourcecontrol-api-openapi.yml
  format: yaml
  label: N8n SourceControl API
  slug: n8n-sourcecontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-sourcecontrol-api-openapi.yml
- filename: n8n-tags-api-openapi.yml
  format: yaml
  label: N8n Tags API
  slug: n8n-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-tags-api-openapi.yml
- filename: n8n-user-api-openapi.yml
  format: yaml
  label: N8n User API
  slug: n8n-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-user-api-openapi.yml
- filename: n8n-variables-api-openapi.yml
  format: yaml
  label: N8n Variables API
  slug: n8n-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-variables-api-openapi.yml
- filename: n8n-workflow-api-openapi.yml
  format: yaml
  label: N8n Workflow API
  slug: n8n-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-workflow-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.n8n.io/connect/n8n-api/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: N8N Scopes
name_suffix: OAuth Scopes
note: n8n's public REST API authenticates with API keys, not OAuth; these are the provider's documented API-key scopes, available on Enterprise instances (non-Enterprise keys have full access). The same scope vocabulary governs what a scoped key may do, and the instance-level MCP server applies scope selection at OAuth consent (n8n 2.32). resource:action format.
overview: 'n8n publishes 67 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the n8n API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: n8n
provider_slug: n8n
schemes: []
scope_count: 67
scope_names:
- communityPackage:install
- communityPackage:list
- communityPackage:uninstall
- communityPackage:update
- credential:create
- credential:read
- credential:list
- credential:update
- credential:delete
- credential:move
- dataTable:create
- dataTable:read
- dataTable:list
- dataTable:update
- dataTable:delete
- dataTableColumn:create
- dataTableColumn:read
- dataTableColumn:update
- dataTableColumn:delete
- dataTableRow:create
- dataTableRow:read
- dataTableRow:update
- dataTableRow:delete
- dataTableRow:upsert
- execution:read
- execution:list
- execution:retry
- execution:stop
- execution:delete
- executionTags:list
- executionTags:update
- folder:create
- folder:read
- folder:list
- folder:update
- folder:delete
- insights:read
- project:create
- project:list
- project:update
- project:delete
- securityAudit:generate
- sourceControl:pull
- tag:create
- tag:read
- tag:list
- tag:update
- tag:delete
- user:create
- user:read
- user:list
- user:changeRole
- user:enforceMfa
- user:delete
- variable:create
- variable:list
- variable:update
- variable:delete
- workflow:create
- workflow:read
- workflow:list
- workflow:update
- workflow:delete
- workflow:move
- workflow:activate
- workflowTags:list
- workflowTags:update
scopes:
- description: Install a community node package on the instance.
  flows: []
  scope: communityPackage:install
- description: List installed community node packages.
  flows: []
  scope: communityPackage:list
- description: Uninstall a community node package.
  flows: []
  scope: communityPackage:uninstall
- description: Update an installed community node package.
  flows: []
  scope: communityPackage:update
- description: Create credentials.
  flows: []
  scope: credential:create
- description: Retrieve a credential and its data schema.
  flows: []
  scope: credential:read
- description: List credentials.
  flows: []
  scope: credential:list
- description: Update a credential.
  flows: []
  scope: credential:update
- description: Delete a credential.
  flows: []
  scope: credential:delete
- description: Transfer a credential to another project.
  flows: []
  scope: credential:move
- description: Create a data table.
  flows: []
  scope: dataTable:create
- description: Retrieve a data table.
  flows: []
  scope: dataTable:read
- description: List data tables.
  flows: []
  scope: dataTable:list
- description: Update a data table's metadata.
  flows: []
  scope: dataTable:update
- description: Delete a data table.
  flows: []
  scope: dataTable:delete
- description: Add a column to a data table.
  flows: []
  scope: dataTableColumn:create
- description: Retrieve a data table column.
  flows: []
  scope: dataTableColumn:read
- description: Update a data table column.
  flows: []
  scope: dataTableColumn:update
- description: Delete a data table column.
  flows: []
  scope: dataTableColumn:delete
- description: Insert rows into a data table.
  flows: []
  scope: dataTableRow:create
- description: Read rows from a data table.
  flows: []
  scope: dataTableRow:read
- description: Update existing rows in a data table.
  flows: []
  scope: dataTableRow:update
- description: Delete rows from a data table.
  flows: []
  scope: dataTableRow:delete
- description: Update an existing row
  flows: []
  scope: dataTableRow:upsert
- description: Retrieve an execution and its details.
  flows: []
  scope: execution:read
- description: List executions.
  flows: []
  scope: execution:list
- description: Retry a failed execution.
  flows: []
  scope: execution:retry
- description: Stop a running execution.
  flows: []
  scope: execution:stop
- description: Delete an execution.
  flows: []
  scope: execution:delete
- description: Read the annotation tags assigned to an execution.
  flows: []
  scope: executionTags:list
- description: Update the annotation tags assigned to an execution.
  flows: []
  scope: executionTags:update
- description: Create a folder in a project.
  flows: []
  scope: folder:create
- description: Retrieve a folder.
  flows: []
  scope: folder:read
- description: List folders in a project.
  flows: []
  scope: folder:list
- description: Update a folder.
  flows: []
  scope: folder:update
- description: Delete a folder.
  flows: []
  scope: folder:delete
- description: Read instance insights data (execution counts
  flows: []
  scope: insights:read
- description: Create a project.
  flows: []
  scope: project:create
- description: List projects.
  flows: []
  scope: project:list
- description: Update a project.
  flows: []
  scope: project:update
- description: Delete a project.
  flows: []
  scope: project:delete
- description: Generate a security audit report for the instance.
  flows: []
  scope: securityAudit:generate
- description: Pull changes from the connected source control repository.
  flows: []
  scope: sourceControl:pull
- description: Create a tag in the global tag registry.
  flows: []
  scope: tag:create
- description: Retrieve a tag.
  flows: []
  scope: tag:read
- description: List tags.
  flows: []
  scope: tag:list
- description: Update a tag.
  flows: []
  scope: tag:update
- description: Delete a tag.
  flows: []
  scope: tag:delete
- description: Invite or create users on the instance.
  flows: []
  scope: user:create
- description: Retrieve a user.
  flows: []
  scope: user:read
- description: List users.
  flows: []
  scope: user:list
- description: Change a user's global (instance-level) role.
  flows: []
  scope: user:changeRole
- description: Reserved scope; no /api/v1/ endpoint consumes it.
  flows: []
  scope: user:enforceMfa
- description: Delete a user from the instance.
  flows: []
  scope: user:delete
- description: Create an instance variable.
  flows: []
  scope: variable:create
- description: List instance variables.
  flows: []
  scope: variable:list
- description: Update an instance variable.
  flows: []
  scope: variable:update
- description: Delete an instance variable.
  flows: []
  scope: variable:delete
- description: Create a workflow.
  flows: []
  scope: workflow:create
- description: Retrieve a workflow and its details.
  flows: []
  scope: workflow:read
- description: List workflows.
  flows: []
  scope: workflow:list
- description: Update a workflow.
  flows: []
  scope: workflow:update
- description: Delete
  flows: []
  scope: workflow:delete
- description: Transfer a workflow to another project.
  flows: []
  scope: workflow:move
- description: Activate/deactivate (publish/unpublish) a workflow.
  flows: []
  scope: workflow:activate
- description: Read the tags assigned to a workflow.
  flows: []
  scope: workflowTags:list
- description: Update the tags assigned to a workflow.
  flows: []
  scope: workflowTags:update
slug: n8n-scopes
source_filename: n8n-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\ndocs: https://docs.n8n.io/connect/n8n-api/authentication\nsource: https://docs.n8n.io/connect/n8n-api/authentication.md (fetched 2026-09-03)\nnote: >-\n  n8n's public REST API authenticates with API keys, not OAuth; these are the\n  provider's documented API-key scopes, available on Enterprise instances\n  (non-Enterprise keys have full access). The same scope vocabulary governs\n  what a scoped key may do, and the instance-level MCP server applies scope\n  selection at OAuth consent (n8n 2.32). resource:action format.\nscopes:\n  - {scope: 'communityPackage:install', description: Install a community node package on the instance.}\n  - {scope: 'communityPackage:list', description: List installed community node packages.}\n  - {scope: 'communityPackage:uninstall', description: Uninstall a community node package.}\n  - {scope: 'communityPackage:update', description: Update an installed community node package.}\n  - {scope: 'credential:create',\
  \ description: Create credentials.}\n  - {scope: 'credential:read', description: Retrieve a credential and its data schema.}\n  - {scope: 'credential:list', description: List credentials.}\n  - {scope: 'credential:update', description: Update a credential.}\n  - {scope: 'credential:delete', description: Delete a credential.}\n  - {scope: 'credential:move', description: Transfer a credential to another project.}\n  - {scope: 'dataTable:create', description: Create a data table.}\n  - {scope: 'dataTable:read', description: Retrieve a data table.}\n  - {scope: 'dataTable:list', description: List data tables.}\n  - {scope: 'dataTable:update', description: Update a data table's metadata.}\n  - {scope: 'dataTable:delete', description: Delete a data table.}\n  - {scope: 'dataTableColumn:create', description: Add a column to a data table.}\n  - {scope: 'dataTableColumn:read', description: Retrieve a data table column.}\n  - {scope: 'dataTableColumn:update', description: Update a data table column.}\n\
  \  - {scope: 'dataTableColumn:delete', description: Delete a data table column.}\n  - {scope: 'dataTableRow:create', description: Insert rows into a data table.}\n  - {scope: 'dataTableRow:read', description: Read rows from a data table.}\n  - {scope: 'dataTableRow:update', description: Update existing rows in a data table.}\n  - {scope: 'dataTableRow:delete', description: Delete rows from a data table.}\n  - {scope: 'dataTableRow:upsert', description: Update an existing row, or insert if no row matches.}\n  - {scope: 'execution:read', description: Retrieve an execution and its details.}\n  - {scope: 'execution:list', description: List executions.}\n  - {scope: 'execution:retry', description: Retry a failed execution.}\n  - {scope: 'execution:stop', description: Stop a running execution.}\n  - {scope: 'execution:delete', description: Delete an execution.}\n  - {scope: 'executionTags:list', description: Read the annotation tags assigned to an execution.}\n  - {scope: 'executionTags:update',\
  \ description: Update the annotation tags assigned to an execution.}\n  - {scope: 'folder:create', description: Create a folder in a project.}\n  - {scope: 'folder:read', description: Retrieve a folder.}\n  - {scope: 'folder:list', description: List folders in a project.}\n  - {scope: 'folder:update', description: Update a folder.}\n  - {scope: 'folder:delete', description: Delete a folder.}\n  - {scope: 'insights:read', description: Read instance insights data (execution counts, failure rates, time saved, run time).}\n  - {scope: 'project:create', description: Create a project.}\n  - {scope: 'project:list', description: List projects.}\n  - {scope: 'project:update', description: Update a project.}\n  - {scope: 'project:delete', description: Delete a project.}\n  - {scope: 'securityAudit:generate', description: Generate a security audit report for the instance.}\n  - {scope: 'sourceControl:pull', description: Pull changes from the connected source control repository.}\n  - {scope: 'tag:create',\
  \ description: Create a tag in the global tag registry.}\n  - {scope: 'tag:read', description: Retrieve a tag.}\n  - {scope: 'tag:list', description: List tags.}\n  - {scope: 'tag:update', description: Update a tag.}\n  - {scope: 'tag:delete', description: Delete a tag.}\n  - {scope: 'user:create', description: Invite or create users on the instance.}\n  - {scope: 'user:read', description: Retrieve a user.}\n  - {scope: 'user:list', description: List users.}\n  - {scope: 'user:changeRole', description: Change a user's global (instance-level) role.}\n  - {scope: 'user:enforceMfa', description: Reserved scope; no /api/v1/ endpoint consumes it.}\n  - {scope: 'user:delete', description: Delete a user from the instance.}\n  - {scope: 'variable:create', description: Create an instance variable.}\n  - {scope: 'variable:list', description: List instance variables.}\n  - {scope: 'variable:update', description: Update an instance variable.}\n  - {scope: 'variable:delete', description: Delete an\
  \ instance variable.}\n  - {scope: 'workflow:create', description: Create a workflow.}\n  - {scope: 'workflow:read', description: Retrieve a workflow and its details.}\n  - {scope: 'workflow:list', description: List workflows.}\n  - {scope: 'workflow:update', description: Update a workflow.}\n  - {scope: 'workflow:delete', description: Delete, archive, or unarchive a workflow.}\n  - {scope: 'workflow:move', description: Transfer a workflow to another project.}\n  - {scope: 'workflow:activate', description: Activate/deactivate (publish/unpublish) a workflow.}\n  - {scope: 'workflowTags:list', description: Read the tags assigned to a workflow.}\n  - {scope: 'workflowTags:update', description: Update the tags assigned to a workflow.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/scopes/n8n-scopes.yml
summary_line: 67 scopes
tags:
- Agents
- Artificial Intelligence
- Integration
- Workflows
- Automation
- Low Code
token_urls: []
---
