---
api_specs:
- filename: companycam-openapi-original.yml
  format: yaml
  label: CompanyCam Core API (v2)
  slug: companycam-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-openapi-original.yml
authorization_urls:
- https://app.companycam.com/oauth/authorize
description: ''
docs: https://docs.companycam.com/docs/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Companycam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CompanyCam publishes 54 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CompanyCam API on a user''s behalf.


  Tokens are issued from https://app.companycam.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CompanyCam
provider_slug: companycam
schemes:
- flows:
  - authorizationUrl: https://app.companycam.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.companycam.com/oauth/token
    tokenUrl: https://app.companycam.com/oauth/token
  introspection_endpoint: https://app.companycam.com/oauth/introspect
  name: OAuth2
  pkce: S256
  registration_endpoint: https://app.companycam.com/oauth/register
  revocation_endpoint: https://app.companycam.com/oauth/revoke
  source: https://app.companycam.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 54
scope_names:
- read
- write
- destroy
- projects:read
- projects:write
- projects:destroy
- photos:read
- photos:write
- photos:destroy
- videos:read
- videos:write
- videos:destroy
- comments:read
- comments:write
- comments:destroy
- users:read
- users:write
- users:destroy
- companies:read
- companies:write
- documents:read
- documents:write
- documents:destroy
- labels:read
- labels:write
- labels:destroy
- tags:read
- tags:write
- tags:destroy
- webhooks:read
- webhooks:write
- webhooks:destroy
- task_lists:read
- task_lists:write
- task_lists:destroy
- project_tasks:read
- project_tasks:write
- project_tasks:destroy
- checklists:read
- checklists:write
- checklists:destroy
- assigned_users:read
- assigned_users:write
- assigned_users:destroy
- collaborators:read
- invitations:read
- invitations:write
- pages:read
- groups:read
- groups:write
- groups:destroy
- project_groups:read
- project_groups:write
- project_groups:destroy
scopes:
- description: Global read access across all resources
  flows: []
  scope: read
- description: Global write (create/update) access across all resources
  flows: []
  scope: write
- description: Global delete access across all resources
  flows: []
  scope: destroy
- description: Read projects
  flows: []
  scope: projects:read
- description: Create and update projects
  flows: []
  scope: projects:write
- description: Delete projects
  flows: []
  scope: projects:destroy
- description: Read photos
  flows: []
  scope: photos:read
- description: Upload and update photos
  flows: []
  scope: photos:write
- description: Delete photos
  flows: []
  scope: photos:destroy
- description: Read videos
  flows: []
  scope: videos:read
- description: Upload and update videos
  flows: []
  scope: videos:write
- description: Delete videos
  flows: []
  scope: videos:destroy
- description: Read comments
  flows: []
  scope: comments:read
- description: Create and update comments
  flows: []
  scope: comments:write
- description: Delete comments
  flows: []
  scope: comments:destroy
- description: Read users
  flows: []
  scope: users:read
- description: Create and update users
  flows: []
  scope: users:write
- description: Delete users
  flows: []
  scope: users:destroy
- description: Read company details
  flows: []
  scope: companies:read
- description: Update company details
  flows: []
  scope: companies:write
- description: Read project documents
  flows: []
  scope: documents:read
- description: Upload and update project documents
  flows: []
  scope: documents:write
- description: Delete project documents
  flows: []
  scope: documents:destroy
- description: Read project labels
  flows: []
  scope: labels:read
- description: Add project labels
  flows: []
  scope: labels:write
- description: Delete project labels
  flows: []
  scope: labels:destroy
- description: Read tags
  flows: []
  scope: tags:read
- description: Create and update tags
  flows: []
  scope: tags:write
- description: Delete tags
  flows: []
  scope: tags:destroy
- description: Read webhooks
  flows: []
  scope: webhooks:read
- description: Create and update webhooks
  flows: []
  scope: webhooks:write
- description: Delete webhooks
  flows: []
  scope: webhooks:destroy
- description: Read task/checklist lists
  flows: []
  scope: task_lists:read
- description: Create and update task lists
  flows: []
  scope: task_lists:write
- description: Delete task lists
  flows: []
  scope: task_lists:destroy
- description: Read project tasks
  flows: []
  scope: project_tasks:read
- description: Create and update project tasks
  flows: []
  scope: project_tasks:write
- description: Delete project tasks
  flows: []
  scope: project_tasks:destroy
- description: Read checklists
  flows: []
  scope: checklists:read
- description: Create checklists on projects
  flows: []
  scope: checklists:write
- description: Delete checklists
  flows: []
  scope: checklists:destroy
- description: Read users assigned to projects
  flows: []
  scope: assigned_users:read
- description: Assign users to projects
  flows: []
  scope: assigned_users:write
- description: Remove assigned users from projects
  flows: []
  scope: assigned_users:destroy
- description: Read project collaborators
  flows: []
  scope: collaborators:read
- description: Read project invitations
  flows: []
  scope: invitations:read
- description: Create project collaboration invitations
  flows: []
  scope: invitations:write
- description: Read pages
  flows: []
  scope: pages:read
- description: Read groups
  flows: []
  scope: groups:read
- description: Create and update groups
  flows: []
  scope: groups:write
- description: Delete groups
  flows: []
  scope: groups:destroy
- description: Read project groups
  flows: []
  scope: project_groups:read
- description: Manage project groups
  flows: []
  scope: project_groups:write
- description: Remove project groups
  flows: []
  scope: project_groups:destroy
slug: companycam-scopes
source_filename: companycam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.companycam.com/.well-known/oauth-authorization-server\ndocs: https://docs.companycam.com/docs/oauth\nnotes: >-\n  CompanyCam OAuth 2.0 authorization-code flow (with refresh tokens and PKCE\n  S256). Scopes are space-delimited. The docs highlight three coarse scopes\n  (read, write, destroy); the RFC 8414 authorization-server metadata publishes a\n  much larger per-resource scope set (resource:action), enumerated below verbatim\n  from scopes_supported.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://app.companycam.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.companycam.com/oauth/authorize\n    tokenUrl: https://app.companycam.com/oauth/token\n    refreshUrl: https://app.companycam.com/oauth/token\n  pkce: S256\n  revocation_endpoint: https://app.companycam.com/oauth/revoke\n  introspection_endpoint: https://app.companycam.com/oauth/introspect\n\
  \  registration_endpoint: https://app.companycam.com/oauth/register\nscopes:\n- {scope: read, description: Global read access across all resources}\n- {scope: write, description: Global write (create/update) access across all resources}\n- {scope: destroy, description: Global delete access across all resources}\n- {scope: 'projects:read', description: Read projects}\n- {scope: 'projects:write', description: Create and update projects}\n- {scope: 'projects:destroy', description: Delete projects}\n- {scope: 'photos:read', description: Read photos}\n- {scope: 'photos:write', description: Upload and update photos}\n- {scope: 'photos:destroy', description: Delete photos}\n- {scope: 'videos:read', description: Read videos}\n- {scope: 'videos:write', description: Upload and update videos}\n- {scope: 'videos:destroy', description: Delete videos}\n- {scope: 'comments:read', description: Read comments}\n- {scope: 'comments:write', description: Create and update comments}\n- {scope: 'comments:destroy',\
  \ description: Delete comments}\n- {scope: 'users:read', description: Read users}\n- {scope: 'users:write', description: Create and update users}\n- {scope: 'users:destroy', description: Delete users}\n- {scope: 'companies:read', description: Read company details}\n- {scope: 'companies:write', description: Update company details}\n- {scope: 'documents:read', description: Read project documents}\n- {scope: 'documents:write', description: Upload and update project documents}\n- {scope: 'documents:destroy', description: Delete project documents}\n- {scope: 'labels:read', description: Read project labels}\n- {scope: 'labels:write', description: Add project labels}\n- {scope: 'labels:destroy', description: Delete project labels}\n- {scope: 'tags:read', description: Read tags}\n- {scope: 'tags:write', description: Create and update tags}\n- {scope: 'tags:destroy', description: Delete tags}\n- {scope: 'webhooks:read', description: Read webhooks}\n- {scope: 'webhooks:write', description: Create\
  \ and update webhooks}\n- {scope: 'webhooks:destroy', description: Delete webhooks}\n- {scope: 'task_lists:read', description: Read task/checklist lists}\n- {scope: 'task_lists:write', description: Create and update task lists}\n- {scope: 'task_lists:destroy', description: Delete task lists}\n- {scope: 'project_tasks:read', description: Read project tasks}\n- {scope: 'project_tasks:write', description: Create and update project tasks}\n- {scope: 'project_tasks:destroy', description: Delete project tasks}\n- {scope: 'checklists:read', description: Read checklists}\n- {scope: 'checklists:write', description: Create checklists on projects}\n- {scope: 'checklists:destroy', description: Delete checklists}\n- {scope: 'assigned_users:read', description: Read users assigned to projects}\n- {scope: 'assigned_users:write', description: Assign users to projects}\n- {scope: 'assigned_users:destroy', description: Remove assigned users from projects}\n- {scope: 'collaborators:read', description: Read\
  \ project collaborators}\n- {scope: 'invitations:read', description: Read project invitations}\n- {scope: 'invitations:write', description: Create project collaboration invitations}\n- {scope: 'pages:read', description: Read pages}\n- {scope: 'groups:read', description: Read groups}\n- {scope: 'groups:write', description: Create and update groups}\n- {scope: 'groups:destroy', description: Delete groups}\n- {scope: 'project_groups:read', description: Read project groups}\n- {scope: 'project_groups:write', description: Manage project groups}\n- {scope: 'project_groups:destroy', description: Remove project groups}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/scopes/companycam-scopes.yml
summary_line: 54 scopes · authorizationCode
tags:
- Company
- Construction
- Photos
- Field Service
- Project Management
- Contractors
- Documentation
- Webhooks
token_urls:
- https://app.companycam.com/oauth/token
---
