---
api_specs:
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-files-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-projects-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-component-sets-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-comments-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-comments-api-openapi.yml
- filename: figma-components-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-components-api-openapi.yml
- filename: figma-library-analytics-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-library-analytics-api-openapi.yml
- filename: figma-users-api-openapi.yml
  format: yaml
  label: Figma Users API
  slug: figma-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-users-api-openapi.yml
- filename: figma-ai-usage-api-openapi.yml
  format: yaml
  label: Figma AI Usage API
  slug: figma-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-ai-usage-api-openapi.yml
- filename: figma-comment-reactions-api-openapi.yml
  format: yaml
  label: Figma Comment Reactions API
  slug: figma-comment-reactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-comment-reactions-api-openapi.yml
- filename: figma-developer-logs-api-openapi.yml
  format: yaml
  label: Figma Developer Logs API
  slug: figma-developer-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-developer-logs-api-openapi.yml
- filename: figma-folders-api-openapi.yml
  format: yaml
  label: Figma Folders API
  slug: figma-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-folders-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-styles-api-openapi.yml
- filename: figma-variables-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-variables-api-openapi.yml
- filename: figma-webhooks-api-openapi.yml
  format: yaml
  label: Figma Webhooks API
  slug: figma-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-webhooks-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-teams-api-openapi.yml
- filename: figma-o-embed-api-openapi.yml
  format: yaml
  label: Figma o Embed API
  slug: figma-o-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/figma/openapi/figma-o-embed-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.figma.com/docs/rest-api/scopes/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Figma Scopes
name_suffix: OAuth Scopes
note: Scopes apply to personal access tokens and OAuth 2 tokens and do not supersede file/team/org permissions. The file_read scope is deprecated for OAuth 2 tokens. The Figma MCP server handles its own OAuth flow and does not use REST API scopes. in_spec marks scopes declared in the oauth2 securitySchemes of openapi/.
overview: 'Figma publishes 31 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Figma API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Figma
provider_slug: figma
schemes: []
scope_count: 31
scope_names:
- current_user:read
- file_comments:read
- file_comments:write
- file_content:read
- file_duplicate:write
- file_dev_resources:read
- file_dev_resources:write
- file_metadata:read
- file_variables:read
- file_variables:write
- file_versions:read
- files:read
- folder_metadata:read
- folders:read
- folders:write
- library_analytics:read
- library_assets:read
- library_content:read
- org:activity_log_read
- org:ai_metering_usage_read
- org:developer_log_read
- org:discovery_read
- project_metadata:read
- projects:read
- selections:read
- team_library_content:read
- team_members:write
- teams:read
- teams:write
- webhooks:read
- webhooks:write
scopes:
- description: Read your name, email, and profile image.
  flows: []
  scope: current_user:read
- description: Read the comments for files.
  flows: []
  scope: file_comments:read
- description: Post and delete comments and comment reactions in files.
  flows: []
  scope: file_comments:write
- description: Read the contents of files, such as nodes and the editor type.
  flows: []
  scope: file_content:read
- description: Duplicate files into folders. Available only to private OAuth apps in an Enterprise plan.
  flows: []
  scope: file_duplicate:write
- description: Read dev resources in files.
  flows: []
  scope: file_dev_resources:read
- description: Write dev resources to files.
  flows: []
  scope: file_dev_resources:write
- description: Read metadata of files.
  flows: []
  scope: file_metadata:read
- description: 'Read variables in files. Note: Enterprise plan only.'
  flows: []
  scope: file_variables:read
- description: 'Write variables and collections in files. Note: Enterprise plan only.'
  flows: []
  scope: file_variables:write
- description: Read the version history for files you can access.
  flows: []
  scope: file_versions:read
- description: Deprecated . Read files, folders, users, versions, comments, components, styles, and webhooks. While this scope will continue to work, it's highly recommended you use the granular scopes Figma provides. Because files:read is extremely permissive, more limited scopes such as file_content:read and file_comments:read provide enhanced security and stability by reducing the surface of access to your files.
  flows: []
  scope: files:read
- description: Read metadata of folders. This is the folders-era equivalent of project_metadata:read and is used by the GET folder metadata endpoint .
  flows: []
  scope: folder_metadata:read
- description: List folders and files in folders. This is the folders-era equivalent of projects:read and is used by the folders endpoints .
  flows: []
  scope: folders:read
- description: Create folders. Available only to private OAuth apps in an Enterprise plan.
  flows: []
  scope: folders:write
- description: 'Read your design system analytics. Note: Enterprise plan only.'
  flows: []
  scope: library_analytics:read
- description: Read data of individual published components and styles.
  flows: []
  scope: library_assets:read
- description: Read published components and styles of files.
  flows: []
  scope: library_content:read
- description: 'Read organization activity logs . Note: Enterprise plan only. Must be an organization admin.'
  flows: []
  scope: org:activity_log_read
- description: 'Read organization AI usage . Note: Enterprise plan only. Must be an organization admin.'
  flows: []
  scope: org:ai_metering_usage_read
- description: 'Read organization developer logs . Note: Enterprise plan with Governance+ only. Must be an organization admin.'
  flows: []
  scope: org:developer_log_read
- description: 'Read text event data in the organization. Note: Enterprise plans with Governance+ only. Must be an organization admin.'
  flows: []
  scope: org:discovery_read
- description: Deprecated in favor of folder_metadata:read . Read metadata of projects (now "folders"). Existing tokens continue to work.
  flows: []
  scope: project_metadata:read
- description: Deprecated in favor of folders:read . List projects (now "folders") and files in projects. Existing tokens continue to work.
  flows: []
  scope: projects:read
- description: Read most recent selection in files you can access.
  flows: []
  scope: selections:read
- description: Read published components and styles of teams.
  flows: []
  scope: team_library_content:read
- description: Invite members to teams. Available only to private OAuth apps in an Enterprise plan.
  flows: []
  scope: team_members:write
- description: Read team metadata. Available only to private OAuth apps in Professional, Organization, and Enterprise plans.
  flows: []
  scope: teams:read
- description: Create teams. Available only to private OAuth apps in an Enterprise plan.
  flows: []
  scope: teams:write
- description: Read metadata of webhooks.
  flows: []
  scope: webhooks:read
- description: Create and manage webhooks.
  flows: []
  scope: webhooks:write
slug: figma-scopes
source_filename: figma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\nsource: https://developers.figma.com/docs/rest-api/scopes/\ndocs: https://developers.figma.com/docs/rest-api/scopes/\nnote: Scopes apply to personal access tokens and OAuth 2 tokens and do not supersede file/team/org permissions.\n  The file_read scope is deprecated for OAuth 2 tokens. The Figma MCP server handles its own OAuth flow\n  and does not use REST API scopes. in_spec marks scopes declared in the oauth2 securitySchemes of openapi/.\nspec_only_scopes: []\nscopes:\n- name: current_user:read\n  description: Read your name, email, and profile image.\n  deprecated: false\n  in_spec: true\n- name: file_comments:read\n  description: Read the comments for files.\n  deprecated: false\n  in_spec: true\n- name: file_comments:write\n  description: Post and delete comments and comment reactions in files.\n  deprecated: false\n  in_spec: true\n- name: file_content:read\n  description: Read the contents of files, such as nodes and the editor\
  \ type.\n  deprecated: false\n  in_spec: true\n- name: file_duplicate:write\n  description: Duplicate files into folders. Available only to private OAuth apps in an Enterprise plan.\n  deprecated: false\n  in_spec: false\n- name: file_dev_resources:read\n  description: Read dev resources in files.\n  deprecated: false\n  in_spec: true\n- name: file_dev_resources:write\n  description: Write dev resources to files.\n  deprecated: false\n  in_spec: true\n- name: file_metadata:read\n  description: Read metadata of files.\n  deprecated: false\n  in_spec: true\n- name: file_variables:read\n  description: 'Read variables in files. Note: Enterprise plan only.'\n  deprecated: false\n  in_spec: true\n- name: file_variables:write\n  description: 'Write variables and collections in files. Note: Enterprise plan only.'\n  deprecated: false\n  in_spec: true\n- name: file_versions:read\n  description: Read the version history for files you can access.\n  deprecated: false\n  in_spec: true\n- name: files:read\n\
  \  description: Deprecated . Read files, folders, users, versions, comments, components, styles, and webhooks.\n    While this scope will continue to work, it's highly recommended you use the granular scopes Figma\n    provides. Because files:read is extremely permissive, more limited scopes such as file_content:read\n    and file_comments:read provide enhanced security and stability by reducing the surface of access to\n    your files.\n  deprecated: true\n  in_spec: true\n- name: folder_metadata:read\n  description: Read metadata of folders. This is the folders-era equivalent of project_metadata:read and\n    is used by the GET folder metadata endpoint .\n  deprecated: false\n  in_spec: true\n- name: folders:read\n  description: List folders and files in folders. This is the folders-era equivalent of projects:read\n    and is used by the folders endpoints .\n  deprecated: false\n  in_spec: true\n- name: folders:write\n  description: Create folders. Available only to private OAuth apps\
  \ in an Enterprise plan.\n  deprecated: false\n  in_spec: false\n- name: library_analytics:read\n  description: 'Read your design system analytics. Note: Enterprise plan only.'\n  deprecated: false\n  in_spec: true\n- name: library_assets:read\n  description: Read data of individual published components and styles.\n  deprecated: false\n  in_spec: true\n- name: library_content:read\n  description: Read published components and styles of files.\n  deprecated: false\n  in_spec: true\n- name: org:activity_log_read\n  description: 'Read organization activity logs . Note: Enterprise plan only. Must be an organization\n    admin.'\n  deprecated: false\n  in_spec: true\n- name: org:ai_metering_usage_read\n  description: 'Read organization AI usage . Note: Enterprise plan only. Must be an organization admin.'\n  deprecated: false\n  in_spec: false\n- name: org:developer_log_read\n  description: 'Read organization developer logs . Note: Enterprise plan with Governance+ only. Must be\n    an organization\
  \ admin.'\n  deprecated: false\n  in_spec: false\n- name: org:discovery_read\n  description: 'Read text event data in the organization. Note: Enterprise plans with Governance+ only.\n    Must be an organization admin.'\n  deprecated: false\n  in_spec: false\n- name: project_metadata:read\n  description: Deprecated in favor of folder_metadata:read . Read metadata of projects (now \"folders\").\n    Existing tokens continue to work.\n  deprecated: true\n  in_spec: true\n- name: projects:read\n  description: Deprecated in favor of folders:read . List projects (now \"folders\") and files in projects.\n    Existing tokens continue to work.\n  deprecated: true\n  in_spec: true\n- name: selections:read\n  description: Read most recent selection in files you can access.\n  deprecated: false\n  in_spec: false\n- name: team_library_content:read\n  description: Read published components and styles of teams.\n  deprecated: false\n  in_spec: true\n- name: team_members:write\n  description: Invite members\
  \ to teams. Available only to private OAuth apps in an Enterprise plan.\n  deprecated: false\n  in_spec: false\n- name: teams:read\n  description: Read team metadata. Available only to private OAuth apps in Professional, Organization,\n    and Enterprise plans.\n  deprecated: false\n  in_spec: false\n- name: teams:write\n  description: Create teams. Available only to private OAuth apps in an Enterprise plan.\n  deprecated: false\n  in_spec: false\n- name: webhooks:read\n  description: Read metadata of webhooks.\n  deprecated: false\n  in_spec: true\n- name: webhooks:write\n  description: Create and manage webhooks.\n  deprecated: false\n  in_spec: true\n"
source_yaml_url: https://artifacts.apis.io/figma/scopes/figma-scopes.yml
summary_line: 31 scopes
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
- Figma
token_bound: false
token_urls: []
---
