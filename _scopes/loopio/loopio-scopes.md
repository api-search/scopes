---
api_specs:
- filename: loopio-asynchronous-api-openapi.yml
  format: yaml
  label: Loopio Asynchronous API
  slug: loopio-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-asynchronous-api-openapi.yml
- filename: loopio-crm-api-openapi.yml
  format: yaml
  label: Loopio CRM API
  slug: loopio-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-crm-api-openapi.yml
- filename: loopio-custom-project-fields-api-openapi.yml
  format: yaml
  label: Loopio Custom Project Fields API
  slug: loopio-custom-project-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-custom-project-fields-api-openapi.yml
- filename: loopio-customers-api-openapi.yml
  format: yaml
  label: Loopio Customers API
  slug: loopio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-customers-api-openapi.yml
- filename: loopio-files-api-openapi.yml
  format: yaml
  label: Loopio Files API
  slug: loopio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-files-api-openapi.yml
- filename: loopio-library-entries-api-openapi.yml
  format: yaml
  label: Loopio Library Entries API
  slug: loopio-library-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-library-entries-api-openapi.yml
- filename: loopio-merge-variables-api-openapi.yml
  format: yaml
  label: Loopio Merge Variables API
  slug: loopio-merge-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-merge-variables-api-openapi.yml
- filename: loopio-project-templates-api-openapi.yml
  format: yaml
  label: Loopio Project Templates API
  slug: loopio-project-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-project-templates-api-openapi.yml
- filename: loopio-projects-api-openapi.yml
  format: yaml
  label: Loopio Projects API
  slug: loopio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-projects-api-openapi.yml
- filename: loopio-roles-api-openapi.yml
  format: yaml
  label: Loopio Roles API
  slug: loopio-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-roles-api-openapi.yml
- filename: loopio-stacks-api-openapi.yml
  format: yaml
  label: Loopio Stacks API
  slug: loopio-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-stacks-api-openapi.yml
- filename: loopio-tags-api-openapi.yml
  format: yaml
  label: Loopio Tags API
  slug: loopio-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-tags-api-openapi.yml
- filename: loopio-teams-api-openapi.yml
  format: yaml
  label: Loopio Teams API
  slug: loopio-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-teams-api-openapi.yml
- filename: loopio-users-api-openapi.yml
  format: yaml
  label: Loopio Users API
  slug: loopio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-users-api-openapi.yml
- filename: loopio-webhooks-api-openapi.yml
  format: yaml
  label: Loopio Webhooks API
  slug: loopio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.loopio.com/docs/loopio-api/c56ffe1fdae3e-getting-started-with-the-loopio-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Loopio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Loopio publishes 52 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Loopio API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Loopio
provider_slug: loopio
schemes: []
scope_count: 52
scope_names:
- appLoopioManaged:delete
- appLoopioManaged:read
- appLoopioManaged:write
- businessUnit:read
- config.cloudStorage:read
- contentIntegration:read
- crm:delete
- crm:read
- crm:write
- customProjectField:delete
- customProjectField:read
- customProjectField:write
- customer.info:read
- documentContent:read
- file:delete
- file:read
- file:write
- library:delete
- library:read
- library:write
- mcp.prompts:all
- mcp.resources:all
- mcp.tools:all
- mergeVariable:delete
- mergeVariable:read
- mergeVariable:write
- metrics:write
- msDynamics:delete
- msDynamics:read
- msDynamics:write
- notification.msDynamics:write
- pitchPartner:all
- project.participant:read
- project.participant:write
- project:delete
- project:read
- project:write
- role:read
- salesforce:read
- salesforce:write
- scim.group:read
- scim.group:write
- scim.user:read
- scim.user:write
- unifiedAnswer:all
- user:delete
- user:read
- user:write
- webhook:delete
- webhook:read
- webhook:write
- zendesk:write
scopes:
- description: ''
  flows: []
  scope: appLoopioManaged:delete
- description: ''
  flows: []
  scope: appLoopioManaged:read
- description: ''
  flows: []
  scope: appLoopioManaged:write
- description: ''
  flows: []
  scope: businessUnit:read
- description: ''
  flows: []
  scope: config.cloudStorage:read
- description: ''
  flows: []
  scope: contentIntegration:read
- description: ''
  flows: []
  scope: crm:delete
- description: List CRM opportunities linked to projects
  flows:
  - authorizationCode
  - clientCredentials
  scope: crm:read
- description: Link CRM opportunities to projects
  flows:
  - authorizationCode
  - clientCredentials
  scope: crm:write
- description: ''
  flows: []
  scope: customProjectField:delete
- description: ''
  flows: []
  scope: customProjectField:read
- description: ''
  flows: []
  scope: customProjectField:write
- description: View customer information
  flows:
  - authorizationCode
  - clientCredentials
  scope: customer.info:read
- description: ''
  flows: []
  scope: documentContent:read
- description: Delete files
  flows:
  - authorizationCode
  - clientCredentials
  scope: file:delete
- description: Download files and view file information
  flows:
  - authorizationCode
  - clientCredentials
  scope: file:read
- description: ''
  flows: []
  scope: file:write
- description: Delete Library Entries
  flows:
  - authorizationCode
  - clientCredentials
  scope: library:delete
- description: List Library Entries and stacks, view Library Entries and Entry data
  flows:
  - authorizationCode
  - clientCredentials
  scope: library:read
- description: Create and update Library Entries and Entry data
  flows:
  - authorizationCode
  - clientCredentials
  scope: library:write
- description: ''
  flows: []
  scope: mcp.prompts:all
- description: ''
  flows: []
  scope: mcp.resources:all
- description: ''
  flows: []
  scope: mcp.tools:all
- description: Delete Merge Variables
  flows:
  - authorizationCode
  - clientCredentials
  scope: mergeVariable:delete
- description: View Merge Variables
  flows:
  - authorizationCode
  - clientCredentials
  scope: mergeVariable:read
- description: Create/Edit Merge Variables
  flows:
  - authorizationCode
  - clientCredentials
  scope: mergeVariable:write
- description: ''
  flows: []
  scope: metrics:write
- description: ''
  flows: []
  scope: msDynamics:delete
- description: ''
  flows: []
  scope: msDynamics:read
- description: ''
  flows: []
  scope: msDynamics:write
- description: ''
  flows: []
  scope: notification.msDynamics:write
- description: ''
  flows: []
  scope: pitchPartner:all
- description: List participants of a project
  flows:
  - authorizationCode
  - clientCredentials
  scope: project.participant:read
- description: Update participant information
  flows:
  - authorizationCode
  - clientCredentials
  scope: project.participant:write
- description: Delete a Project
  flows:
  - authorizationCode
  - clientCredentials
  scope: project:delete
- description: List Projects, view Project data and source documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: project:read
- description: Create and update Projects, Project data, and source documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: project:write
- description: List user assignable roles
  flows:
  - authorizationCode
  - clientCredentials
  scope: role:read
- description: ''
  flows: []
  scope: salesforce:read
- description: ''
  flows: []
  scope: salesforce:write
- description: ''
  flows: []
  scope: scim.group:read
- description: ''
  flows: []
  scope: scim.group:write
- description: ''
  flows: []
  scope: scim.user:read
- description: ''
  flows: []
  scope: scim.user:write
- description: ''
  flows: []
  scope: unifiedAnswer:all
- description: ''
  flows: []
  scope: user:delete
- description: List users, view user information
  flows:
  - authorizationCode
  - clientCredentials
  scope: user:read
- description: Update user information
  flows:
  - authorizationCode
  - clientCredentials
  scope: user:write
- description: Delete webhook subscriptions
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook:delete
- description: View webhook subscriptions
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook:read
- description: Create & edit webhook subscriptions
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook:write
- description: ''
  flows: []
  scope: zendesk:write
slug: loopio-scopes
source_filename: loopio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://api.loopio.com/.well-known/oauth-authorization-server\ndocs: https://developer.loopio.com/docs/loopio-api/c56ffe1fdae3e-getting-started-with-the-loopio-api\nderived_from:\n- openapi/loopio-openapi.yaml\n- well-known/loopio-oauth-authorization-server.json\nscheme: loopio_auth\nflows:\n- authorizationCode\n- clientCredentials\ntoken_endpoint: https://api.loopio.com/oauth2/access_token\nauthorization_endpoint: https://api.loopio.com/oauth2/authorize\ndelimiter: space (URL-encoded as +)\ncounts:\n  declared_in_openapi: 22\n  advertised_by_authorization_server: 51\n  applied_to_operations: 26\n  advertised_but_not_in_openapi: 30\nnotes:\n- The authorization server advertises 51 scopes; the published OpenAPI declares only 22. The 30 extra\n  scopes describe surfaces Loopio operates but does not document in the public contract.\n- Scopes are fixed at App creation time and cannot be edited afterwards.\n- businessUnit:write\
  \ is applied to bulkAssignBusinessUnitUsers but is NOT declared in the securityScheme\n  scopes map — an in-spec inconsistency.\nscopes:\n- scope: appLoopioManaged:delete\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: appLoopioManaged:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: appLoopioManaged:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: businessUnit:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: config.cloudStorage:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: contentIntegration:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: crm:delete\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: crm:read\n  description: List\
  \ CRM opportunities linked to projects\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - listCRMProjects\n- scope: crm:write\n  description: Link CRM opportunities to projects\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - createOpportunityLink\n- scope: customProjectField:delete\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - deleteCustomProjectField\n- scope: customProjectField:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 2\n  operations:\n  - getCustomProjectField\n  - listCustomProjectFields\n- scope: customProjectField:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 2\n  operations:\n  - createCustomProjectField\n\
  \  - updateCustomProjectField\n- scope: customer.info:read\n  description: View customer information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: false\n  operation_count: 2\n  operations:\n  - getCustomer\n  - getCustomerActiveLanguages\n- scope: documentContent:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: file:delete\n  description: Delete files\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - deleteFile\n- scope: file:read\n  description: Download files and view file information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - showFile\n- scope: file:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count:\
  \ 0\n- scope: library:delete\n  description: Delete Library Entries\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - deleteLibraryEntry\n- scope: library:read\n  description: List Library Entries and stacks, view Library Entries and Entry data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 7\n  operations:\n  - getLibraryEntry\n  - getLibraryEntryFiles\n  - getLibraryEntryHistories\n  - getLibraryEntryHistory\n  - getTags\n  - listLibraryEntries\n  - listStacks\n- scope: library:write\n  description: Create and update Library Entries and Entry data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 6\n  operations:\n  - bulkCreateLibraryEntries\n  - createLibraryEntry\n  - deleteLibraryEntryAttachment\n\
  \  - replaceLibraryEntryAttachment\n  - updateLibraryEntry\n  - uploadLibraryEntryAttachment\n- scope: mcp.prompts:all\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: mcp.resources:all\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: mcp.tools:all\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: mergeVariable:delete\n  description: Delete Merge Variables\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - deleteMergeVariable\n- scope: mergeVariable:read\n  description: View Merge Variables\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 4\n  operations:\n  - getMergeVariable\n  - getMergeVariableHistory\n  - getMergeVariableValuesForProject\n  -\
  \ listMergeVariables\n- scope: mergeVariable:write\n  description: Create/Edit Merge Variables\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 3\n  operations:\n  - createMergeVariable\n  - setMergeVariableValuesForProject\n  - updateMergeVariable\n- scope: metrics:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: msDynamics:delete\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: msDynamics:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: msDynamics:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: notification.msDynamics:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: pitchPartner:all\n  in_openapi: false\n  advertised_by_authorization_server:\
  \ true\n  operation_count: 0\n- scope: project.participant:read\n  description: List participants of a project\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - getProjectParticipants\n- scope: project.participant:write\n  description: Update participant information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - updateProjectParticipants\n- scope: project:delete\n  description: Delete a Project\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - deleteProject\n- scope: project:read\n  description: List Projects, view Project data and source documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server:\
  \ true\n  operation_count: 15\n  operations:\n  - getCustomProjectFieldValuesForProject\n  - getMergeVariableValuesForProject\n  - getProject\n  - getProjectEntry\n  - getProjectEntryAttachments\n  - getProjectSection\n  - getProjectSubQuestion\n  - getProjectSummary\n  - getProjectSummaryList\n  - listProjectEntries\n  - listProjectSections\n  - listProjectSourceDocuments\n  - listProjectSubSections\n  - listProjectTemplates\n  - listProjects\n- scope: project:write\n  description: Create and update Projects, Project data, and source documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 18\n  operations:\n  - addProjectSourceDocument\n  - createProject\n  - createProjectEntry\n  - createProjectFromTemplate\n  - createProjectSection\n  - createProjectSubSection\n  - deleteProjectEntry\n  - deleteProjectEntryAttachment\n  - deleteProjectSection\n  - deleteProjectSubSection\n  - replaceProjectEntryAttachment\n\
  \  - setCustomProjectFieldValuesForProject\n  - setMergeVariableValuesForProject\n  - updateProject\n  - updateProjectEntry\n  - updateProjectSection\n  - updateProjectSubSection\n  - uploadProjectEntryAttachment\n- scope: role:read\n  description: List user assignable roles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 2\n  operations:\n  - getRole\n  - listRoles\n- scope: salesforce:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: salesforce:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: scim.group:read\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: scim.group:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: scim.user:read\n  in_openapi: false\n  advertised_by_authorization_server:\
  \ true\n  operation_count: 0\n- scope: scim.user:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: unifiedAnswer:all\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: user:delete\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count: 0\n- scope: user:read\n  description: List users, view user information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 5\n  operations:\n  - getTeam\n  - getUser\n  - identifyUser\n  - listTeams\n  - listUsers\n- scope: user:write\n  description: Update user information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 7\n  operations:\n  - bulkAssignRole\n  - bulkAssignUsersToTeams\n  - bulkRemoveUsers\n  - bulkResendActivationEmail\n  - bulkUserDisableByEmail\n\
  \  - createUser\n  - updateUser\n- scope: webhook:delete\n  description: Delete webhook subscriptions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 1\n  operations:\n  - cancelWebhookSubscription\n- scope: webhook:read\n  description: View webhook subscriptions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 2\n  operations:\n  - getWebhookSubscription\n  - listWebhookSubscriptions\n- scope: webhook:write\n  description: Create & edit webhook subscriptions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  in_openapi: true\n  advertised_by_authorization_server: true\n  operation_count: 3\n  operations:\n  - createWebhookSubscription\n  - refreshWebhookSigningSecret\n  - updateWebhookSubscription\n- scope: zendesk:write\n  in_openapi: false\n  advertised_by_authorization_server: true\n  operation_count:\
  \ 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/scopes/loopio-scopes.yml
summary_line: 52 scopes
tags:
- Company
- RFP
- Proposals
- Response Management
- Content Library
- Sales Enablement
- Questionnaires
- Compliance
- Collaboration
- Documents
- Webhook
- Software-as-a-Service
token_urls: []
---
