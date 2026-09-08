---
api_specs:
- filename: atlassian-jira-fields-api-openapi.yml
  format: yaml
  label: Atlassian Jira Fields API
  slug: atlassian-jira-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-fields-api-openapi.yml
- filename: atlassian-jira-issue-comments-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Comments API
  slug: atlassian-jira-issue-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-comments-api-openapi.yml
- filename: atlassian-jira-issue-search-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Search API
  slug: atlassian-jira-issue-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-search-api-openapi.yml
- filename: atlassian-jira-issue-transitions-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Transitions API
  slug: atlassian-jira-issue-transitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-transitions-api-openapi.yml
- filename: atlassian-jira-issue-worklogs-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Worklogs API
  slug: atlassian-jira-issue-worklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-worklogs-api-openapi.yml
- filename: atlassian-jira-issues-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issues API
  slug: atlassian-jira-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issues-api-openapi.yml
- filename: atlassian-jira-projects-api-openapi.yml
  format: yaml
  label: Atlassian Jira Projects API
  slug: atlassian-jira-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-projects-api-openapi.yml
- filename: atlassian-jira-users-api-openapi.yml
  format: yaml
  label: Atlassian Jira Users API
  slug: atlassian-jira-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-users-api-openapi.yml
- filename: atlassian-jira-platform-openapi.json
  format: json
  label: Atlassian Jira Cloud Platform REST API v3
  slug: atlassian-jira-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-platform-openapi.json
- filename: atlassian-jira-software-openapi.json
  format: json
  label: Jira Software Cloud API
  slug: atlassian-jira-software-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-software-openapi.json
- filename: atlassian-jira-service-management-openapi.json
  format: json
  label: Jira Service Management REST API
  slug: atlassian-jira-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-service-management-openapi.json
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Atlassian Jira Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Atlassian Jira publishes 281 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Atlassian Jira API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atlassian Jira
provider_slug: atlassian-jira
schemes:
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-fields-api-openapi.yml
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-issue-comments-api-openapi.yml
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-issue-search-api-openapi.yml
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-issue-transitions-api-openapi.yml
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-issue-worklogs-api-openapi.yml
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-issues-api-openapi.yml
- description: OAuth2 scopes for Jira
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-platform-openapi.json
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-projects-api-openapi.yml
- description: OAuth2 scopes for Jira
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-service-management-openapi.json
- description: OAuth2 scopes for Jira
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-software-openapi.json
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  source: openapi/atlassian-jira-users-api-openapi.yml
scope_count: 281
scope_names:
- delete:async-task:jira
- delete:attachment:jira
- delete:avatar:jira
- delete:board-scope.admin:jira-software
- delete:build-info:jira
- delete:comment.property:jira
- delete:comment:jira
- delete:dashboard.property:jira
- delete:dashboard:jira
- delete:deployment-info:jira
- delete:dev-info:jira
- delete:feature-flag-info:jira
- delete:field-configuration-scheme:jira
- delete:field-configuration:jira
- delete:field.option:jira
- delete:field:jira
- delete:filter.column:jira
- delete:filter:jira
- delete:group:jira
- delete:issue-link-type:jira
- delete:issue-link:jira
- delete:issue-type-scheme:jira
- delete:issue-type-screen-scheme:jira
- delete:issue-type.property:jira
- delete:issue-type:jira
- delete:issue-worklog.property:jira
- delete:issue-worklog:jira
- delete:issue.property:jira
- delete:issue.remote-link:jira
- delete:issue:jira
- delete:organization.property:jira-service-management
- delete:organization.user:jira-service-management
- delete:organization:jira-service-management
- delete:permission-scheme:jira
- delete:permission:jira
- delete:project-category:jira
- delete:project-role:jira
- delete:project-version:jira
- delete:project.avatar:jira
- delete:project.component:jira
- delete:project.property:jira
- delete:project:jira
- delete:remote-link-info:jira
- delete:request.feedback:jira-service-management
- delete:request.notification:jira-service-management
- delete:request.participant:jira-service-management
- delete:requesttype.property:jira-service-management
- delete:screen-scheme:jira
- delete:screen-tab:jira
- delete:screen:jira
- delete:screenable-field:jira
- delete:security:jira
- delete:servicedesk.customer:jira-service-management
- delete:servicedesk.organization:jira-service-management
- delete:servicedesk.property:jira-service-management
- delete:sprint:jira-software
- delete:user-configuration:jira
- delete:user.property:jira
- delete:webhook:jira
- delete:workflow-scheme:jira
- delete:workflow.property:jira
- delete:workflow:jira
- manage:jira-configuration
- manage:jira-project
- manage:jira-webhook
- manage:servicedesk-customer
- read:app-data:jira
- read:application-role:jira
- read:attachment:jira
- read:audit-log:jira
- read:avatar:jira
- read:board-scope.admin:jira-software
- read:board-scope:jira-software
- read:build-info:jira
- read:build:jira-software
- read:comment.property:jira
- read:comment:jira
- read:custom-field-contextual-configuration:jira
- read:customer:jira-service-management
- read:dashboard.property:jira
- read:dashboard:jira
- read:deployment-info:jira
- read:deployment:jira-software
- read:dev-info:jira
- read:email-address:jira
- read:epic:jira-software
- read:feature-flag-info:jira
- read:feature-flag:jira-software
- read:field-configuration-scheme:jira
- read:field-configuration:jira
- read:field.default-value:jira
- read:field.option:jira
- read:field.options:jira
- read:field:jira
- read:filter.column:jira
- read:filter.default-share-scope:jira
- read:filter:jira
- read:group:jira
- read:instance-configuration:jira
- read:issue-details:jira
- read:issue-event:jira
- read:issue-field-values:jira
- read:issue-link-type:jira
- read:issue-link:jira
- read:issue-meta:jira
- read:issue-security-level:jira
- read:issue-security-scheme:jira
- read:issue-status:jira
- read:issue-type-hierarchy:jira
- read:issue-type-scheme:jira
- read:issue-type-screen-scheme:jira
- read:issue-type.property:jira
- read:issue-type:jira
- read:issue-worklog.property:jira
- read:issue-worklog:jira
- read:issue.changelog:jira
- read:issue.property:jira
- read:issue.remote-link:jira
- read:issue.time-tracking:jira
- read:issue.transition:jira
- read:issue.vote:jira
- read:issue.votes:jira
- read:issue.watcher:jira
- read:issue:jira
- read:issue:jira-software
- read:jira-expressions:jira
- read:jira-user
- read:jira-work
- read:jql:jira
- read:knowledgebase:jira-service-management
- read:label:jira
- read:license:jira
- read:mail-logs.connectivity:jira-service-management
- read:mail-logs.processing:jira-service-management
- read:notification-scheme:jira
- read:organization.property:jira-service-management
- read:organization.user:jira-service-management
- read:organization:jira-service-management
- read:permission-scheme:jira
- read:permission:jira
- read:priority:jira
- read:project-category:jira
- read:project-role:jira
- read:project-type:jira
- read:project-version:jira
- read:project.avatar:jira
- read:project.component:jira
- read:project.email:jira
- read:project.feature:jira
- read:project.property:jira
- read:project:jira
- read:queue:jira-service-management
- read:remote-link-info:jira
- read:remote-link:jira-software
- read:request.action:jira-service-management
- read:request.approval:jira-service-management
- read:request.attachment:jira-service-management
- read:request.comment:jira-service-management
- read:request.feedback:jira-service-management
- read:request.notification:jira-service-management
- read:request.participant:jira-service-management
- read:request.sla:jira-service-management
- read:request.status:jira-service-management
- read:request:jira-service-management
- read:requesttype.property:jira-service-management
- read:requesttype:jira-service-management
- read:resolution:jira
- read:role:jira
- read:screen-field:jira
- read:screen-scheme:jira
- read:screen-tab:jira
- read:screen:jira
- read:screenable-field:jira
- read:security:jira
- read:servicedesk-request
- read:servicedesk.customer:jira-service-management
- read:servicedesk.organization:jira-service-management
- read:servicedesk.property:jira-service-management
- read:servicedesk:jira-service-management
- read:source-code:jira-software
- read:sprint:jira-software
- read:status:jira
- read:user-configuration:jira
- read:user.columns:jira
- read:user.property:jira
- read:user:jira
- read:webhook:jira
- read:workflow-scheme:jira
- read:workflow.property:jira
- read:workflow:jira
- send:notification:jira
- validate:jql:jira
- write:app-data:jira
- write:attachment:jira
- write:avatar:jira
- write:board-scope.admin:jira-software
- write:board-scope:jira-software
- write:build-info:jira
- write:build:jira-software
- write:comment.property:jira
- write:comment:jira
- write:custom-field-contextual-configuration:jira
- write:customer:jira-service-management
- write:dashboard.property:jira
- write:dashboard:jira
- write:deployment-info:jira
- write:deployment:jira-software
- write:dev-info:jira
- write:epic:jira-software
- write:feature-flag-info:jira
- write:feature-flag:jira-software
- write:field-configuration-scheme:jira
- write:field-configuration:jira
- write:field.default-value:jira
- write:field.option:jira
- write:field:jira
- write:filter.column:jira
- write:filter.default-share-scope:jira
- write:filter:jira
- write:group:jira
- write:instance-configuration:jira
- write:issue-link-type:jira
- write:issue-link:jira
- write:issue-type-scheme:jira
- write:issue-type-screen-scheme:jira
- write:issue-type.property:jira
- write:issue-type:jira
- write:issue-worklog.property:jira
- write:issue-worklog:jira
- write:issue.property:jira
- write:issue.remote-link:jira
- write:issue.time-tracking:jira
- write:issue.vote:jira
- write:issue.watcher:jira
- write:issue:jira
- write:issue:jira-software
- write:jira-work
- write:organization.property:jira-service-management
- write:organization.user:jira-service-management
- write:organization:jira-service-management
- write:permission-scheme:jira
- write:permission:jira
- write:project-category:jira
- write:project-role:jira
- write:project-version:jira
- write:project.avatar:jira
- write:project.component:jira
- write:project.email:jira
- write:project.feature:jira
- write:project.property:jira
- write:project:jira
- write:remote-link-info:jira
- write:remote-link:jira-software
- write:request.approval:jira-service-management
- write:request.attachment:jira-service-management
- write:request.comment:jira-service-management
- write:request.feedback:jira-service-management
- write:request.notification:jira-service-management
- write:request.participant:jira-service-management
- write:request.status:jira-service-management
- write:request:jira-service-management
- write:requesttype.property:jira-service-management
- write:requesttype:jira-service-management
- write:screen-scheme:jira
- write:screen-tab:jira
- write:screen:jira
- write:screenable-field:jira
- write:security:jira
- write:servicedesk-request
- write:servicedesk.customer:jira-service-management
- write:servicedesk.organization:jira-service-management
- write:servicedesk.property:jira-service-management
- write:servicedesk:jira-service-management
- write:source-code:jira-software
- write:sprint:jira-software
- write:user-configuration:jira
- write:user.property:jira
- write:webhook:jira
- write:workflow-scheme:jira
- write:workflow.property:jira
- write:workflow:jira
scopes:
- description: Delete asynchronous task.
  flows:
  - authorizationCode
  scope: delete:async-task:jira
- description: Delete issue attachments.
  flows:
  - authorizationCode
  scope: delete:attachment:jira
- description: Delete system and custom avatars.
  flows:
  - authorizationCode
  scope: delete:avatar:jira
- description: Remove board configuration, features, and properties.
  flows:
  - authorizationCode
  scope: delete:board-scope.admin:jira-software
- description: Delete build information
  flows:
  - authorizationCode
  scope: delete:build-info:jira
- description: Delete issue comment properties.
  flows:
  - authorizationCode
  scope: delete:comment.property:jira
- description: Delete issue comments.
  flows:
  - authorizationCode
  scope: delete:comment:jira
- description: Delete dashboard properties.
  flows:
  - authorizationCode
  scope: delete:dashboard.property:jira
- description: Delete dashboards.
  flows:
  - authorizationCode
  scope: delete:dashboard:jira
- description: Delete deployment information
  flows:
  - authorizationCode
  scope: delete:deployment-info:jira
- description: Delete development information
  flows:
  - authorizationCode
  scope: delete:dev-info:jira
- description: Delete feature flag information
  flows:
  - authorizationCode
  scope: delete:feature-flag-info:jira
- description: Delete field configuration schemes.
  flows:
  - authorizationCode
  scope: delete:field-configuration-scheme:jira
- description: Delete field configurations.
  flows:
  - authorizationCode
  scope: delete:field-configuration:jira
- description: Delete field options.
  flows:
  - authorizationCode
  scope: delete:field.option:jira
- description: Delete fields.
  flows:
  - authorizationCode
  scope: delete:field:jira
- description: Delete filter columns.
  flows:
  - authorizationCode
  scope: delete:filter.column:jira
- description: Delete filters.
  flows:
  - authorizationCode
  scope: delete:filter:jira
- description: Delete user groups.
  flows:
  - authorizationCode
  scope: delete:group:jira
- description: Delete issue link types.
  flows:
  - authorizationCode
  scope: delete:issue-link-type:jira
- description: Delete issue links.
  flows:
  - authorizationCode
  scope: delete:issue-link:jira
- description: Delete issue type schemes.
  flows:
  - authorizationCode
  scope: delete:issue-type-scheme:jira
- description: Delete issue type screen schemes.
  flows:
  - authorizationCode
  scope: delete:issue-type-screen-scheme:jira
- description: Delete issue type properties.
  flows:
  - authorizationCode
  scope: delete:issue-type.property:jira
- description: Delete issue types.
  flows:
  - authorizationCode
  scope: delete:issue-type:jira
- description: Delete issue worklog properties.
  flows:
  - authorizationCode
  scope: delete:issue-worklog.property:jira
- description: Delete issue worklogs.
  flows:
  - authorizationCode
  scope: delete:issue-worklog:jira
- description: Delete issue properties.
  flows:
  - authorizationCode
  scope: delete:issue.property:jira
- description: Delete issue remote links.
  flows:
  - authorizationCode
  scope: delete:issue.remote-link:jira
- description: Delete issues.
  flows:
  - authorizationCode
  scope: delete:issue:jira
- description: Allows the app to delete organisation entity properties
  flows:
  - authorizationCode
  scope: delete:organization.property:jira-service-management
- description: Allows the app to remove members from organisations
  flows:
  - authorizationCode
  scope: delete:organization.user:jira-service-management
- description: Allows the app to delete organisations
  flows:
  - authorizationCode
  scope: delete:organization:jira-service-management
- description: Delete permission schemes.
  flows:
  - authorizationCode
  scope: delete:permission-scheme:jira
- description: Delete permissions.
  flows:
  - authorizationCode
  scope: delete:permission:jira
- description: Delete project categories.
  flows:
  - authorizationCode
  scope: delete:project-category:jira
- description: Delete project roles.
  flows:
  - authorizationCode
  scope: delete:project-role:jira
- description: Delete project versions.
  flows:
  - authorizationCode
  scope: delete:project-version:jira
- description: Delete project avatars.
  flows:
  - authorizationCode
  scope: delete:project.avatar:jira
- description: Delete project components.
  flows:
  - authorizationCode
  scope: delete:project.component:jira
- description: Delete project properties.
  flows:
  - authorizationCode
  scope: delete:project.property:jira
- description: Delete projects and their details, such as issue types, project lead, and avatars.
  flows:
  - authorizationCode
  scope: delete:project:jira
- description: Delete remote link information
  flows:
  - authorizationCode
  scope: delete:remote-link-info:jira
- description: Allows the app to remove feedback data from requests
  flows:
  - authorizationCode
  scope: delete:request.feedback:jira-service-management
- description: Allows the app to remove the subscription status of the user from requests
  flows:
  - authorizationCode
  scope: delete:request.notification:jira-service-management
- description: Allows the app to remove participants (user) data from requests
  flows:
  - authorizationCode
  scope: delete:request.participant:jira-service-management
- description: Allows the app to delete request type entity properties
  flows:
  - authorizationCode
  scope: delete:requesttype.property:jira-service-management
- description: Delete screen schemes.
  flows:
  - authorizationCode
  scope: delete:screen-scheme:jira
- description: Delete screen tabs.
  flows:
  - authorizationCode
  scope: delete:screen-tab:jira
- description: Delete screens.
  flows:
  - authorizationCode
  scope: delete:screen:jira
- description: Delete screenable fields.
  flows:
  - authorizationCode
  scope: delete:screenable-field:jira
- description: Delete security information
  flows:
  - authorizationCode
  scope: delete:security:jira
- description: Allows the app the delete customers from service desks
  flows:
  - authorizationCode
  scope: delete:servicedesk.customer:jira-service-management
- description: Allows the app the delete organisations from service desks
  flows:
  - authorizationCode
  scope: delete:servicedesk.organization:jira-service-management
- description: Allows the app to delete service desk entity properties
  flows:
  - authorizationCode
  scope: delete:servicedesk.property:jira-service-management
- description: Delete sprints and their properties.
  flows:
  - authorizationCode
  scope: delete:sprint:jira-software
- description: Delete user configurations.
  flows:
  - authorizationCode
  scope: delete:user-configuration:jira
- description: Delete user properties.
  flows:
  - authorizationCode
  scope: delete:user.property:jira
- description: Delete webhooks.
  flows:
  - authorizationCode
  scope: delete:webhook:jira
- description: Delete workflow schemes.
  flows:
  - authorizationCode
  scope: delete:workflow-scheme:jira
- description: Delete workflow properties.
  flows:
  - authorizationCode
  scope: delete:workflow.property:jira
- description: Delete workflows.
  flows:
  - authorizationCode
  scope: delete:workflow:jira
- description: Configure Jira settings that require the Jira administrators permission, for example, create projects and custom fields, view workflows, manage issue link types.
  flows:
  - authorizationCode
  scope: manage:jira-configuration
- description: Manage Jira projects
  flows:
  - authorizationCode
  scope: manage:jira-project
- description: Manage Jira webhooks. Enables an OAuth app to register and unregister dynamic webhooks in Jira. It also provides for fetching of registered webhooks.
  flows:
  - authorizationCode
  scope: manage:jira-webhook
- description: Manage Jira Service Management customers and organizations | Create, manage and delete customers and organizations.<br>Add and remove customers and organizations from service desks.
  flows:
  - authorizationCode
  scope: manage:servicedesk-customer
- description: Read app data.
  flows:
  - authorizationCode
  scope: read:app-data:jira
- description: View application roles.
  flows:
  - authorizationCode
  scope: read:application-role:jira
- description: View issue attachments.
  flows:
  - authorizationCode
  scope: read:attachment:jira
- description: View audit logs.
  flows:
  - authorizationCode
  scope: read:audit-log:jira
- description: View system and custom avatars.
  flows:
  - authorizationCode
  scope: read:avatar:jira
- description: View configuration, features, filters, project, properties and quick filters related to the given board.
  flows:
  - authorizationCode
  scope: read:board-scope.admin:jira-software
- description: View board and issues from a board, view issues from a backlog and view reports and versions.
  flows:
  - authorizationCode
  scope: read:board-scope:jira-software
- description: Read build information
  flows:
  - authorizationCode
  scope: read:build-info:jira
- description: View builds.
  flows:
  - authorizationCode
  scope: read:build:jira-software
- description: View issue comment properties.
  flows:
  - authorizationCode
  scope: read:comment.property:jira
- description: View issue comments.
  flows:
  - authorizationCode
  scope: read:comment:jira
- description: Read custom field contextual configurations.
  flows:
  - authorizationCode
  scope: read:custom-field-contextual-configuration:jira
- description: Allows the app to read customer accounts information
  flows:
  - authorizationCode
  scope: read:customer:jira-service-management
- description: View dashboard properties.
  flows:
  - authorizationCode
  scope: read:dashboard.property:jira
- description: View dashboards.
  flows:
  - authorizationCode
  scope: read:dashboard:jira
- description: Read deployment information
  flows:
  - authorizationCode
  scope: read:deployment-info:jira
- description: View deployments.
  flows:
  - authorizationCode
  scope: read:deployment:jira-software
- description: Read development information
  flows:
  - authorizationCode
  scope: read:dev-info:jira
- description: View email addresses of all users regardless of the user's profile visibility settings.
  flows:
  - authorizationCode
  scope: read:email-address:jira
- description: View and search for epics, view issues related to an epic and issues without an epic.
  flows:
  - authorizationCode
  scope: read:epic:jira-software
- description: Read feature flag information
  flows:
  - authorizationCode
  scope: read:feature-flag-info:jira
- description: View feature flags.
  flows:
  - authorizationCode
  scope: read:feature-flag:jira-software
- description: View field configuration schemes.
  flows:
  - authorizationCode
  scope: read:field-configuration-scheme:jira
- description: Read field configurations.
  flows:
  - authorizationCode
  scope: read:field-configuration:jira
- description: View field default values.
  flows:
  - authorizationCode
  scope: read:field.default-value:jira
- description: View field options.
  flows:
  - authorizationCode
  scope: read:field.option:jira
- description: Read field options.
  flows:
  - authorizationCode
  scope: read:field.options:jira
- description: View fields.
  flows:
  - authorizationCode
  scope: read:field:jira
- description: View filter columns.
  flows:
  - authorizationCode
  scope: read:filter.column:jira
- description: View filter default share scopes.
  flows:
  - authorizationCode
  scope: read:filter.default-share-scope:jira
- description: View filters.
  flows:
  - authorizationCode
  scope: read:filter:jira
- description: View user groups.
  flows:
  - authorizationCode
  scope: read:group:jira
- description: View instance configurations.
  flows:
  - authorizationCode
  scope: read:instance-configuration:jira
- description: View issue details.
  flows:
  - authorizationCode
  scope: read:issue-details:jira
- description: Read issue events.
  flows:
  - authorizationCode
  scope: read:issue-event:jira
- description: View issue field valueses.
  flows:
  - authorizationCode
  scope: read:issue-field-values:jira
- description: View issue link types.
  flows:
  - authorizationCode
  scope: read:issue-link-type:jira
- description: View issue links.
  flows:
  - authorizationCode
  scope: read:issue-link:jira
- description: View issue meta.
  flows:
  - authorizationCode
  scope: read:issue-meta:jira
- description: View issue security levels.
  flows:
  - authorizationCode
  scope: read:issue-security-level:jira
- description: View issue security schemes.
  flows:
  - authorizationCode
  scope: read:issue-security-scheme:jira
- description: View issue statuses.
  flows:
  - authorizationCode
  scope: read:issue-status:jira
- description: Read issue type hierarchies.
  flows:
  - authorizationCode
  scope: read:issue-type-hierarchy:jira
- description: View issue type schemes.
  flows:
  - authorizationCode
  scope: read:issue-type-scheme:jira
- description: View issue type screen schemes.
  flows:
  - authorizationCode
  scope: read:issue-type-screen-scheme:jira
- description: View issue type properties.
  flows:
  - authorizationCode
  scope: read:issue-type.property:jira
- description: View issue types.
  flows:
  - authorizationCode
  scope: read:issue-type:jira
- description: View issue worklog properties.
  flows:
  - authorizationCode
  scope: read:issue-worklog.property:jira
- description: View issue worklogs.
  flows:
  - authorizationCode
  scope: read:issue-worklog:jira
- description: View issue changelogs.
  flows:
  - authorizationCode
  scope: read:issue.changelog:jira
- description: View issue properties.
  flows:
  - authorizationCode
  scope: read:issue.property:jira
- description: View issue remote links.
  flows:
  - authorizationCode
  scope: read:issue.remote-link:jira
- description: View issue time trackings.
  flows:
  - authorizationCode
  scope: read:issue.time-tracking:jira
- description: View issue transitions.
  flows:
  - authorizationCode
  scope: read:issue.transition:jira
- description: View issue votes.
  flows:
  - authorizationCode
  scope: read:issue.vote:jira
- description: View issue voteses.
  flows:
  - authorizationCode
  scope: read:issue.votes:jira
- description: View issue watchers.
  flows:
  - authorizationCode
  scope: read:issue.watcher:jira
- description: View issues.
  flows:
  - authorizationCode
  scope: read:issue:jira
- description: View issues, issue estimations and field used for estimations.
  flows:
  - authorizationCode
  scope: read:issue:jira-software
- description: View jira expressions.
  flows:
  - authorizationCode
  scope: read:jira-expressions:jira
- description: Read Jira user
  flows:
  - authorizationCode
  scope: read:jira-user
- description: Read Jira work
  flows:
  - authorizationCode
  scope: read:jira-work
- description: View JQL.
  flows:
  - authorizationCode
  scope: read:jql:jira
- description: Allows the app to search and list KB articles
  flows:
  - authorizationCode
  scope: read:knowledgebase:jira-service-management
- description: View labels.
  flows:
  - authorizationCode
  scope: read:label:jira
- description: View licenses.
  flows:
  - authorizationCode
  scope: read:license:jira
- description: Allows the app to read email connectivity logs
  flows:
  - authorizationCode
  scope: read:mail-logs.connectivity:jira-service-management
- description: Allows the app to read incoming email processing logs
  flows:
  - authorizationCode
  scope: read:mail-logs.processing:jira-service-management
- description: View notification schemes.
  flows:
  - authorizationCode
  scope: read:notification-scheme:jira
- description: Allows the app to read organisation entity properties
  flows:
  - authorizationCode
  scope: read:organization.property:jira-service-management
- description: Allows the app to read organisation membership information
  flows:
  - authorizationCode
  scope: read:organization.user:jira-service-management
- description: Allows the app to read organisation information
  flows:
  - authorizationCode
  scope: read:organization:jira-service-management
- description: View permission schemes.
  flows:
  - authorizationCode
  scope: read:permission-scheme:jira
- description: View permissions.
  flows:
  - authorizationCode
  scope: read:permission:jira
- description: View priorities.
  flows:
  - authorizationCode
  scope: read:priority:jira
- description: View project categories.
  flows:
  - authorizationCode
  scope: read:project-category:jira
- description: View project roles.
  flows:
  - authorizationCode
  scope: read:project-role:jira
- description: View project types.
  flows:
  - authorizationCode
  scope: read:project-type:jira
- description: View project versions.
  flows:
  - authorizationCode
  scope: read:project-version:jira
- description: Read project avatars.
  flows:
  - authorizationCode
  scope: read:project.avatar:jira
- description: View project components.
  flows:
  - authorizationCode
  scope: read:project.component:jira
- description: View project emails.
  flows:
  - authorizationCode
  scope: read:project.email:jira
- description: Read project features.
  flows:
  - authorizationCode
  scope: read:project.feature:jira
- description: View project properties.
  flows:
  - authorizationCode
  scope: read:project.property:jira
- description: View projects.
  flows:
  - authorizationCode
  scope: read:project:jira
- description: Allows the app to list queues
  flows:
  - authorizationCode
  scope: read:queue:jira-service-management
- description: Read remote link information
  flows:
  - authorizationCode
  scope: read:remote-link-info:jira
- description: View remote links.
  flows:
  - authorizationCode
  scope: read:remote-link:jira-software
- description: Allows the app to read which actions can be performed on requests
  flows:
  - authorizationCode
  scope: read:request.action:jira-service-management
- description: Allows the app to read approval data from requests
  flows:
  - authorizationCode
  scope: read:request.approval:jira-service-management
- description: Allows the app to read attachment data from requests
  flows:
  - authorizationCode
  scope: read:request.attachment:jira-service-management
- description: Allows the app to read comment data from requests
  flows:
  - authorizationCode
  scope: read:request.comment:jira-service-management
- description: Allows the app to read feedback data from requests
  flows:
  - authorizationCode
  scope: read:request.feedback:jira-service-management
- description: Allows the app to read the subscription status of the user for requests
  flows:
  - authorizationCode
  scope: read:request.notification:jira-service-management
- description: Allows the app to read participant (user) data from requests
  flows:
  - authorizationCode
  scope: read:request.participant:jira-service-management
- description: Allows the app to read SLA data from requests
  flows:
  - authorizationCode
  scope: read:request.sla:jira-service-management
- description: Allows the app to read status/transition data from requests
  flows:
  - authorizationCode
  scope: read:request.status:jira-service-management
- description: Allows the app to list & search requests
  flows:
  - authorizationCode
  scope: read:request:jira-service-management
- description: Allows the app to read request type desk entity properties
  flows:
  - authorizationCode
  scope: read:requesttype.property:jira-service-management
- description: Allows the app to list & search request types
  flows:
  - authorizationCode
  scope: read:requesttype:jira-service-management
- description: View resolutions.
  flows:
  - authorizationCode
  scope: read:resolution:jira
- description: View roles.
  flows:
  - authorizationCode
  scope: read:role:jira
- description: View screen fields.
  flows:
  - authorizationCode
  scope: read:screen-field:jira
- description: View screen schemes.
  flows:
  - authorizationCode
  scope: read:screen-scheme:jira
- description: View screen tabs.
  flows:
  - authorizationCode
  scope: read:screen-tab:jira
- description: View screens.
  flows:
  - authorizationCode
  scope: read:screen:jira
- description: View screenable fields.
  flows:
  - authorizationCode
  scope: read:screenable-field:jira
- description: Read security information
  flows:
  - authorizationCode
  scope: read:security:jira
- description: Read customer request data, including approvals, attachments, comments, request participants, and status/transitions.<br>Read service desk and request types, including searching for request types and reading request type fields, properties and groups.
  flows:
  - authorizationCode
  scope: read:servicedesk-request
- description: Allows the app the list customers of service desks
  flows:
  - authorizationCode
  scope: read:servicedesk.customer:jira-service-management
- description: Allows the app to list organisations to service desks
  flows:
  - authorizationCode
  scope: read:servicedesk.organization:jira-service-management
- description: Allows the app to read service desk entity properties
  flows:
  - authorizationCode
  scope: read:servicedesk.property:jira-service-management
- description: Allows the app to list & search service desks
  flows:
  - authorizationCode
  scope: read:servicedesk:jira-service-management
- description: View repositories and check if data exists for the supplied properties.
  flows:
  - authorizationCode
  scope: read:source-code:jira-software
- description: View sprints and sprint related issues and properties.
  flows:
  - authorizationCode
  scope: read:sprint:jira-software
- description: View statuses.
  flows:
  - authorizationCode
  scope: read:status:jira
- description: View user configurations.
  flows:
  - authorizationCode
  scope: read:user-configuration:jira
- description: View user columnses.
  flows:
  - authorizationCode
  scope: read:user.columns:jira
- description: View user properties.
  flows:
  - authorizationCode
  scope: read:user.property:jira
- description: View users.
  flows:
  - authorizationCode
  scope: read:user:jira
- description: View webhooks.
  flows:
  - authorizationCode
  scope: read:webhook:jira
- description: View workflow schemes.
  flows:
  - authorizationCode
  scope: read:workflow-scheme:jira
- description: View workflow properties.
  flows:
  - authorizationCode
  scope: read:workflow.property:jira
- description: View workflows.
  flows:
  - authorizationCode
  scope: read:workflow:jira
- description: Send notifications.
  flows:
  - authorizationCode
  scope: send:notification:jira
- description: Validate JQL.
  flows:
  - authorizationCode
  scope: validate:jql:jira
- description: Write app data.
  flows:
  - authorizationCode
  scope: write:app-data:jira
- description: Create and update issue attachments.
  flows:
  - authorizationCode
  scope: write:attachment:jira
- description: Create and update system and custom avatars.
  flows:
  - authorizationCode
  scope: write:avatar:jira
- description: Create board, toggle features and set and delete properties.
  flows:
  - authorizationCode
  scope: write:board-scope.admin:jira-software
- description: Move issues to a backlog and move issues from a backlog to a board.
  flows:
  - authorizationCode
  scope: write:board-scope:jira-software
- description: Write build information
  flows:
  - authorizationCode
  scope: write:build-info:jira
- description: Submit and delete build.
  flows:
  - authorizationCode
  scope: write:build:jira-software
- description: Create and update issue comment properties.
  flows:
  - authorizationCode
  scope: write:comment.property:jira
- description: Create and update issue comments.
  flows:
  - authorizationCode
  scope: write:comment:jira
- description: Save custom field contextual configurations.
  flows:
  - authorizationCode
  scope: write:custom-field-contextual-configuration:jira
- description: Allows the app to create customer accounts (user)
  flows:
  - authorizationCode
  scope: write:customer:jira-service-management
- description: Create and update dashboard properties.
  flows:
  - authorizationCode
  scope: write:dashboard.property:jira
- description: Create and update dashboards.
  flows:
  - authorizationCode
  scope: write:dashboard:jira
- description: Write deployment information
  flows:
  - authorizationCode
  scope: write:deployment-info:jira
- description: Submit and delete deployment.
  flows:
  - authorizationCode
  scope: write:deployment:jira-software
- description: Write development information
  flows:
  - authorizationCode
  scope: write:dev-info:jira
- description: Remove issues from epic, move issues to epic, rank epics and partially update epics. A partial update means that fields not present in the request JSON will not be updated.
  flows:
  - authorizationCode
  scope: write:epic:jira-software
- description: Write feature flag information
  flows:
  - authorizationCode
  scope: write:feature-flag-info:jira
- description: Submit and delete feature flag.
  flows:
  - authorizationCode
  scope: write:feature-flag:jira-software
- description: Create and update field configuration schemes.
  flows:
  - authorizationCode
  scope: write:field-configuration-scheme:jira
- description: Save field configurations.
  flows:
  - authorizationCode
  scope: write:field-configuration:jira
- description: Create and update field default values.
  flows:
  - authorizationCode
  scope: write:field.default-value:jira
- description: Create and update field options.
  flows:
  - authorizationCode
  scope: write:field.option:jira
- description: Create and update fields.
  flows:
  - authorizationCode
  scope: write:field:jira
- description: Create and update filter columns.
  flows:
  - authorizationCode
  scope: write:filter.column:jira
- description: Create and update filter default share scopes.
  flows:
  - authorizationCode
  scope: write:filter.default-share-scope:jira
- description: Create and update filters.
  flows:
  - authorizationCode
  scope: write:filter:jira
- description: Create and update user groups.
  flows:
  - authorizationCode
  scope: write:group:jira
- description: Create and update instance configurations.
  flows:
  - authorizationCode
  scope: write:instance-configuration:jira
- description: Create and update issue link types.
  flows:
  - authorizationCode
  scope: write:issue-link-type:jira
- description: Create and update issue links.
  flows:
  - authorizationCode
  scope: write:issue-link:jira
- description: Create and update issue type schemes.
  flows:
  - authorizationCode
  scope: write:issue-type-scheme:jira
- description: Create and update issue type screen schemes.
  flows:
  - authorizationCode
  scope: write:issue-type-screen-scheme:jira
- description: Create and update issue type properties.
  flows:
  - authorizationCode
  scope: write:issue-type.property:jira
- description: Create and update issue types.
  flows:
  - authorizationCode
  scope: write:issue-type:jira
- description: Create and update issue worklog properties.
  flows:
  - authorizationCode
  scope: write:issue-worklog.property:jira
- description: Create and update issue worklogs.
  flows:
  - authorizationCode
  scope: write:issue-worklog:jira
- description: Create and update issue properties.
  flows:
  - authorizationCode
  scope: write:issue.property:jira
- description: Create and update issue remote links.
  flows:
  - authorizationCode
  scope: write:issue.remote-link:jira
- description: Create and update issue time trackings.
  flows:
  - authorizationCode
  scope: write:issue.time-tracking:jira
- description: Create and update issue votes.
  flows:
  - authorizationCode
  scope: write:issue.vote:jira
- description: Create and update issue watchers.
  flows:
  - authorizationCode
  scope: write:issue.watcher:jira
- description: Create and update issues.
  flows:
  - authorizationCode
  scope: write:issue:jira
- description: Move (rank) issues and update estimation of the issue.
  flows:
  - authorizationCode
  scope: write:issue:jira-software
- description: Write Jira work
  flows:
  - authorizationCode
  scope: write:jira-work
- description: Allows the app to write organisation entity properties
  flows:
  - authorizationCode
  scope: write:organization.property:jira-service-management
- description: Allows the app to add members to organisations
  flows:
  - authorizationCode
  scope: write:organization.user:jira-service-management
- description: Allows the app to create organisations
  flows:
  - authorizationCode
  scope: write:organization:jira-service-management
- description: Create and update permission schemes.
  flows:
  - authorizationCode
  scope: write:permission-scheme:jira
- description: Create and update permissions.
  flows:
  - authorizationCode
  scope: write:permission:jira
- description: Create and update project categories.
  flows:
  - authorizationCode
  scope: write:project-category:jira
- description: Create and update project roles.
  flows:
  - authorizationCode
  scope: write:project-role:jira
- description: Create and update project versions.
  flows:
  - authorizationCode
  scope: write:project-version:jira
- description: Create and update project avatars.
  flows:
  - authorizationCode
  scope: write:project.avatar:jira
- description: Create and update project components.
  flows:
  - authorizationCode
  scope: write:project.component:jira
- description: Create and update project emails.
  flows:
  - authorizationCode
  scope: write:project.email:jira
- description: Save project features.
  flows:
  - authorizationCode
  scope: write:project.feature:jira
- description: Create and update project properties.
  flows:
  - authorizationCode
  scope: write:project.property:jira
- description: Create and update projects.
  flows:
  - authorizationCode
  scope: write:project:jira
- description: Write remote link information
  flows:
  - authorizationCode
  scope: write:remote-link-info:jira
- description: Submit and delete remote link.
  flows:
  - authorizationCode
  scope: write:remote-link:jira-software
- description: Allows the app to act on approvals of requests (e.g approve, deny, …)
  flows:
  - authorizationCode
  scope: write:request.approval:jira-service-management
- description: Allows the app to add attachments to requests
  flows:
  - authorizationCode
  scope: write:request.attachment:jira-service-management
- description: Allows the app to add comments to requests
  flows:
  - authorizationCode
  scope: write:request.comment:jira-service-management
- description: Allows the app to write feedback data on requests
  flows:
  - authorizationCode
  scope: write:request.feedback:jira-service-management
- description: Allows the app to change the subscription status of the user for requests
  flows:
  - authorizationCode
  scope: write:request.notification:jira-service-management
- description: Allows the app to add participants (user) data from requests
  flows:
  - authorizationCode
  scope: write:request.participant:jira-service-management
- description: Allows the app to execute transitions on requests
  flows:
  - authorizationCode
  scope: write:request.status:jira-service-management
- description: Allows the app to create requests
  flows:
  - authorizationCode
  scope: write:request:jira-service-management
- description: Allows the app to write request type entity properties
  flows:
  - authorizationCode
  scope: write:requesttype.property:jira-service-management
- description: Allows the app to create or modify request types
  flows:
  - authorizationCode
  scope: write:requesttype:jira-service-management
- description: Create and update screen schemes.
  flows:
  - authorizationCode
  scope: write:screen-scheme:jira
- description: Create and update screen tabs.
  flows:
  - authorizationCode
  scope: write:screen-tab:jira
- description: Create and update screens.
  flows:
  - authorizationCode
  scope: write:screen:jira
- description: Create and update screenable fields.
  flows:
  - authorizationCode
  scope: write:screenable-field:jira
- description: Write security information
  flows:
  - authorizationCode
  scope: write:security:jira
- description: Create and manage Jira Service Management requests | Create and edit customer requests, including add comments and attachments, approve, share (add request participants), subscribe, and transition.
  flows:
  - authorizationCode
  scope: write:servicedesk-request
- description: Allows the app the add customers to service desks
  flows:
  - authorizationCode
  scope: write:servicedesk.customer:jira-service-management
- description: Allows the app the add organisations to service desks
  flows:
  - authorizationCode
  scope: write:servicedesk.organization:jira-service-management
- description: Allows the app to write service desk entity properties
  flows:
  - authorizationCode
  scope: write:servicedesk.property:jira-service-management
- description: Allows the app the add organisations, customers and request types to service desks
  flows:
  - authorizationCode
  scope: write:servicedesk:jira-service-management
- description: Store and delete development information, delete repository and delete development information entity.
  flows:
  - authorizationCode
  scope: write:source-code:jira-software
- description: Save, move issues to sprints, and change the order of sprints.
  flows:
  - authorizationCode
  scope: write:sprint:jira-software
- description: Create and update user configurations.
  flows:
  - authorizationCode
  scope: write:user-configuration:jira
- description: Create and update user properties.
  flows:
  - authorizationCode
  scope: write:user.property:jira
- description: Create and update webhooks.
  flows:
  - authorizationCode
  scope: write:webhook:jira
- description: Create and update workflow schemes.
  flows:
  - authorizationCode
  scope: write:workflow-scheme:jira
- description: Create and update workflow properties.
  flows:
  - authorizationCode
  scope: write:workflow.property:jira
- description: Create and update workflows.
  flows:
  - authorizationCode
  scope: write:workflow:jira
slug: atlassian-jira-scopes
source_filename: atlassian-jira-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/atlassian-jira-fields-api-openapi.yml, openapi/atlassian-jira-issue-comments-api-openapi.yml,\n  openapi/atlassian-jira-issue-search-api-openapi.yml, openapi/atlassian-jira-issue-transitions-api-openapi.yml,\n  openapi/atlassian-jira-issue-worklogs-api-openapi.yml, openapi/atlassian-jira-issues-api-openapi.yml,\n  openapi/atlassian-jira-platform-openapi.json, openapi/atlassian-jira-projects-api-openapi.yml,\n  openapi/atlassian-jira-service-management-openapi.json, openapi/atlassian-jira-software-openapi.json,\n  openapi/atlassian-jira-users-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/atlassian-jira-fields-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-issue-comments-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-issue-search-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-issue-transitions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-issue-worklogs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n\
  \  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-issues-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-platform-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth2 scopes for Jira\n- name: OAuth2\n  source: openapi/atlassian-jira-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n- name: OAuth2\n  source: openapi/atlassian-jira-service-management-openapi.json\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth2 scopes for Jira\n- name: OAuth2\n  source: openapi/atlassian-jira-software-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: OAuth2 scopes for Jira\n- name: OAuth2\n  source: openapi/atlassian-jira-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\nscopes:\n- scope: delete:async-task:jira\n  description: Delete asynchronous task.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:attachment:jira\n  description: Delete issue attachments.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:avatar:jira\n  description: Delete system and custom avatars.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:board-scope.admin:jira-software\n  description: Remove board configuration, features, and properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:build-info:jira\n  description: Delete build information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:comment.property:jira\n  description: Delete issue comment properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:comment:jira\n  description: Delete issue comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:dashboard.property:jira\n  description:\
  \ Delete dashboard properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:dashboard:jira\n  description: Delete dashboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:deployment-info:jira\n  description: Delete deployment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:dev-info:jira\n  description: Delete development information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:feature-flag-info:jira\n  description: Delete feature flag information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:field-configuration-scheme:jira\n  description: Delete field configuration schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  - scope: delete:field-configuration:jira\n  description: Delete field configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:field.option:jira\n  description: Delete field options.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:field:jira\n  description: Delete fields.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:filter.column:jira\n  description: Delete filter columns.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:filter:jira\n  description: Delete filters.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:group:jira\n  description: Delete user groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-link-type:jira\n\
  \  description: Delete issue link types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-link:jira\n  description: Delete issue links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-type-scheme:jira\n  description: Delete issue type schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-type-screen-scheme:jira\n  description: Delete issue type screen schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-type.property:jira\n  description: Delete issue type properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-type:jira\n  description: Delete issue types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  - scope: delete:issue-worklog.property:jira\n  description: Delete issue worklog properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue-worklog:jira\n  description: Delete issue worklogs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue.property:jira\n  description: Delete issue properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue.remote-link:jira\n  description: Delete issue remote links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:issue:jira\n  description: Delete issues.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:organization.property:jira-service-management\n  description: Allows the app to delete organisation entity properties\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:organization.user:jira-service-management\n  description: Allows the app to remove members from organisations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:organization:jira-service-management\n  description: Allows the app to delete organisations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:permission-scheme:jira\n  description: Delete permission schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:permission:jira\n  description: Delete permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project-category:jira\n  description: Delete project categories.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project-role:jira\n  description: Delete project roles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project-version:jira\n  description: Delete project versions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project.avatar:jira\n  description: Delete project avatars.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project.component:jira\n  description: Delete project components.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project.property:jira\n  description: Delete project properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:project:jira\n  description: Delete projects and their\
  \ details, such as issue types, project lead, and avatars.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:remote-link-info:jira\n  description: Delete remote link information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:request.feedback:jira-service-management\n  description: Allows the app to remove feedback data from requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:request.notification:jira-service-management\n  description: Allows the app to remove the subscription status of the user from requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:request.participant:jira-service-management\n  description: Allows the app to remove participants (user) data from requests\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:requesttype.property:jira-service-management\n  description: Allows the app to delete request type entity properties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:screen-scheme:jira\n  description: Delete screen schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:screen-tab:jira\n  description: Delete screen tabs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:screen:jira\n  description: Delete screens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:screenable-field:jira\n  description: Delete screenable fields.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:security:jira\n\
  \  description: Delete security information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:servicedesk.customer:jira-service-management\n  description: Allows the app the delete customers from service desks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:servicedesk.organization:jira-service-management\n  description: Allows the app the delete organisations from service desks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:servicedesk.property:jira-service-management\n  description: Allows the app to delete service desk entity properties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: delete:sprint:jira-software\n  description: Delete sprints and their properties.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/atlassian-jira-software-openapi.json\n- scope: delete:user-configuration:jira\n  description: Delete user configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:user.property:jira\n  description: Delete user properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:webhook:jira\n  description: Delete webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:workflow-scheme:jira\n  description: Delete workflow schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:workflow.property:jira\n  description: Delete workflow properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: delete:workflow:jira\n  description: Delete workflows.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: manage:jira-configuration\n  description: Configure Jira settings that require the Jira administrators permission, for\n    example, create projects and custom fields, view workflows, manage issue link types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n  - openapi/atlassian-jira-service-management-openapi.json\n  - openapi/atlassian-jira-software-openapi.json\n- scope: manage:jira-project\n  description: Manage Jira projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-fields-api-openapi.yml\n  - openapi/atlassian-jira-issue-comments-api-openapi.yml\n  - openapi/atlassian-jira-issue-search-api-openapi.yml\n  - openapi/atlassian-jira-issue-transitions-api-openapi.yml\n  - openapi/atlassian-jira-issue-worklogs-api-openapi.yml\n  - openapi/atlassian-jira-issues-api-openapi.yml\n  - openapi/atlassian-jira-platform-openapi.json\n  - openapi/atlassian-jira-projects-api-openapi.yml\n\
  \  - openapi/atlassian-jira-service-management-openapi.json\n  - openapi/atlassian-jira-software-openapi.json\n  - openapi/atlassian-jira-users-api-openapi.yml\n- scope: manage:jira-webhook\n  description: Manage Jira webhooks. Enables an OAuth app to register and unregister dynamic\n    webhooks in Jira. It also provides for fetching of registered webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n  - openapi/atlassian-jira-service-management-openapi.json\n  - openapi/atlassian-jira-software-openapi.json\n- scope: manage:servicedesk-customer\n  description: Manage Jira Service Management customers and organizations | Create, manage and\n    delete customers and organizations.<br>Add and remove customers and organizations from service\n    desks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:app-data:jira\n  description: Read app data.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:application-role:jira\n  description: View application roles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:attachment:jira\n  description: View issue attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:audit-log:jira\n  description: View audit logs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:avatar:jira\n  description: View system and custom avatars.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:board-scope.admin:jira-software\n  description: View configuration, features, filters, project, properties and quick filters\n    related to the given board.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope:\
  \ read:board-scope:jira-software\n  description: View board and issues from a board, view issues from a backlog and view reports\n    and versions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:build-info:jira\n  description: Read build information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:build:jira-software\n  description: View builds.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:comment.property:jira\n  description: View issue comment properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:comment:jira\n  description: View issue comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:custom-field-contextual-configuration:jira\n  description: Read custom field contextual\
  \ configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:customer:jira-service-management\n  description: Allows the app to read customer accounts information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:dashboard.property:jira\n  description: View dashboard properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:dashboard:jira\n  description: View dashboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:deployment-info:jira\n  description: Read deployment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:deployment:jira-software\n  description: View deployments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n\
  - scope: read:dev-info:jira\n  description: Read development information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:email-address:jira\n  description: View email addresses of all users regardless of the user's profile visibility\n    settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:epic:jira-software\n  description: View and search for epics, view issues related to an epic and issues without\n    an epic.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:feature-flag-info:jira\n  description: Read feature flag information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:feature-flag:jira-software\n  description: View feature flags.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope:\
  \ read:field-configuration-scheme:jira\n  description: View field configuration schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:field-configuration:jira\n  description: Read field configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:field.default-value:jira\n  description: View field default values.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:field.option:jira\n  description: View field options.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:field.options:jira\n  description: Read field options.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:field:jira\n  description: View fields.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  - scope: read:filter.column:jira\n  description: View filter columns.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:filter.default-share-scope:jira\n  description: View filter default share scopes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:filter:jira\n  description: View filters.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:group:jira\n  description: View user groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:instance-configuration:jira\n  description: View instance configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-details:jira\n  description: View issue details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  \  - openapi/atlassian-jira-software-openapi.json\n- scope: read:issue-event:jira\n  description: Read issue events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-field-values:jira\n  description: View issue field valueses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-link-type:jira\n  description: View issue link types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-link:jira\n  description: View issue links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-meta:jira\n  description: View issue meta.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-security-level:jira\n  description: View issue security levels.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-security-scheme:jira\n  description: View issue security schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-status:jira\n  description: View issue statuses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-type-hierarchy:jira\n  description: Read issue type hierarchies.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-type-scheme:jira\n  description: View issue type schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-type-screen-scheme:jira\n  description: View issue type screen schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-type.property:jira\n  description: View\
  \ issue type properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-type:jira\n  description: View issue types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-worklog.property:jira\n  description: View issue worklog properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue-worklog:jira\n  description: View issue worklogs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.changelog:jira\n  description: View issue changelogs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.property:jira\n  description: View issue properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.remote-link:jira\n\
  \  description: View issue remote links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.time-tracking:jira\n  description: View issue time trackings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.transition:jira\n  description: View issue transitions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.vote:jira\n  description: View issue votes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.votes:jira\n  description: View issue voteses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue.watcher:jira\n  description: View issue watchers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue:jira\n\
  \  description: View issues.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:issue:jira-software\n  description: View issues, issue estimations and field used for estimations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n- scope: read:jira-expressions:jira\n  description: View jira expressions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:jira-user\n  description: Read Jira user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-fields-api-openapi.yml\n  - openapi/atlassian-jira-issue-comments-api-openapi.yml\n  - openapi/atlassian-jira-issue-search-api-openapi.yml\n  - openapi/atlassian-jira-issue-transitions-api-openapi.yml\n  - openapi/atlassian-jira-issue-worklogs-api-openapi.yml\n  - openapi/atlassian-jira-issues-api-openapi.yml\n  - openapi/atlassian-jira-platform-openapi.json\n  - openapi/atlassian-jira-projects-api-openapi.yml\n\
  \  - openapi/atlassian-jira-service-management-openapi.json\n  - openapi/atlassian-jira-software-openapi.json\n  - openapi/atlassian-jira-users-api-openapi.yml\n- scope: read:jira-work\n  description: Read Jira work\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-fields-api-openapi.yml\n  - openapi/atlassian-jira-issue-comments-api-openapi.yml\n  - openapi/atlassian-jira-issue-search-api-openapi.yml\n  - openapi/atlassian-jira-issue-transitions-api-openapi.yml\n  - openapi/atlassian-jira-issue-worklogs-api-openapi.yml\n  - openapi/atlassian-jira-issues-api-openapi.yml\n  - openapi/atlassian-jira-platform-openapi.json\n  - openapi/atlassian-jira-projects-api-openapi.yml\n  - openapi/atlassian-jira-service-management-openapi.json\n  - openapi/atlassian-jira-software-openapi.json\n  - openapi/atlassian-jira-users-api-openapi.yml\n- scope: read:jql:jira\n  description: View JQL.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  \  - openapi/atlassian-jira-software-openapi.json\n- scope: read:knowledgebase:jira-service-management\n  description: Allows the app to search and list KB articles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:label:jira\n  description: View labels.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:license:jira\n  description: View licenses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:mail-logs.connectivity:jira-service-management\n  description: Allows the app to read email connectivity logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:mail-logs.processing:jira-service-management\n  description: Allows the app to read incoming email processing logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n\
  - scope: read:notification-scheme:jira\n  description: View notification schemes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:organization.property:jira-service-management\n  description: Allows the app to read organisation entity properties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:organization.user:jira-service-management\n  description: Allows the app to read organisation membership information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:organization:jira-service-management\n  description: Allows the app to read organisation information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:permission-scheme:jira\n  description: View permission schemes.\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/atlassian-jira-platform-openapi.json\n- scope: read:permission:jira\n  description: View permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:priority:jira\n  description: View priorities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project-category:jira\n  description: View project categories.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project-role:jira\n  description: View project roles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project-type:jira\n  description: View project types.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project-version:jira\n  description: View project versions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  - scope: read:project.avatar:jira\n  description: Read project avatars.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project.component:jira\n  description: View project components.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project.email:jira\n  description: View project emails.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project.feature:jira\n  description: Read project features.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project.property:jira\n  description: View project properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n- scope: read:project:jira\n  description: View projects.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-platform-openapi.json\n\
  \  - openapi/atlassian-jira-software-openapi.json\n- scope: read:queue:jira-service-management\n  description: Allows the app to list queues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-service-management-openapi.json\n- scope: read:remote-link-info:jira\n  description: Read remote link information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-jira-software-openapi.json\n\n\n# --- truncated at 32 KB (56 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/scopes/atlassian-jira-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/scopes/atlassian-jira-scopes.yml
summary_line: 281 scopes · authorizationCode
tags:
- Agile
- Atlassian
- Bug Tracking
- Issue Tracking
- ITSM
- Kanban
- Project Management
- Scrum
- Service Desk
token_urls:
- https://auth.atlassian.com/oauth/token
---
