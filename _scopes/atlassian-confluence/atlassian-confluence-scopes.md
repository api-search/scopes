---
api_specs:
- filename: atlassian-confluence-rest-v2-openapi.json
  format: json
  label: Confluence Cloud REST API v2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/openapi/atlassian-confluence-rest-v2-openapi.json
- filename: atlassian-confluence-rest-v1-openapi.json
  format: json
  label: Confluence Cloud REST API v1
  slug: confluence-cloud-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/openapi/atlassian-confluence-rest-v1-openapi.json
authorization_urls:
- https://auth.atlassian.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Atlassian Confluence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Atlassian Confluence publishes 90 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Atlassian Confluence API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atlassian Confluence
provider_slug: atlassian-confluence
schemes:
- description: This API uses OAuth 2 with the authorizationCode grant flow.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuthDefinitions
  source: openapi/atlassian-confluence-rest-v1-openapi.json
- description: This API uses OAuth 2 with the authorizationCode grant flow.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuthDefinitions
  source: openapi/atlassian-confluence-rest-v2-openapi.json
scope_count: 90
scope_names:
- delete:attachment:confluence
- delete:blogpost:confluence
- delete:comment:confluence
- delete:content:confluence
- delete:custom-content:confluence
- delete:database:confluence
- delete:embed:confluence
- delete:folder:confluence
- delete:page:confluence
- delete:space:confluence
- delete:whiteboard:confluence
- manage:confluence-configuration
- moderate:comment:confluence
- moderate:core-content:confluence
- read:analytics.content:confluence
- read:app-data:confluence
- read:attachment:confluence
- read:audit-log:confluence
- read:blogpost:confluence
- read:comment:confluence
- read:configuration:confluence
- read:confluence-content.all
- read:confluence-content.permission
- read:confluence-content.summary
- read:confluence-groups
- read:confluence-props
- read:confluence-space.summary
- read:confluence-user
- read:content-details:confluence
- read:content.metadata:confluence
- read:content.permission:confluence
- read:content.property:confluence
- read:content.restriction:confluence
- read:content:confluence
- read:custom-content:confluence
- read:database:confluence
- read:email-address:confluence
- read:embed:confluence
- read:folder:confluence
- read:group:confluence
- read:hierarchical-content:confluence
- read:inlinetask:confluence
- read:label:confluence
- read:page:confluence
- read:relation:confluence
- read:space-details:confluence
- read:space.permission:confluence
- read:space.property:confluence
- read:space.setting:confluence
- read:space:confluence
- read:task:confluence
- read:template:confluence
- read:user.property:confluence
- read:user:confluence
- read:watcher:confluence
- read:whiteboard:confluence
- readonly:content.attachment:confluence
- search:confluence
- write:app-data:confluence
- write:attachment:confluence
- write:audit-log:confluence
- write:blogpost:confluence
- write:comment:confluence
- write:configuration:confluence
- write:confluence-content
- write:confluence-file
- write:confluence-groups
- write:confluence-props
- write:confluence-space
- write:content.property:confluence
- write:content.restriction:confluence
- write:content:confluence
- write:custom-content:confluence
- write:database:confluence
- write:embed:confluence
- write:folder:confluence
- write:group:confluence
- write:inlinetask:confluence
- write:label:confluence
- write:page:confluence
- write:relation:confluence
- write:space.permission:confluence
- write:space.property:confluence
- write:space.setting:confluence
- write:space:confluence
- write:task:confluence
- write:template:confluence
- write:user.property:confluence
- write:watcher:confluence
- write:whiteboard:confluence
scopes:
- description: Delete attachments.
  flows:
  - authorizationCode
  scope: delete:attachment:confluence
- description: Delete blogposts.
  flows:
  - authorizationCode
  scope: delete:blogpost:confluence
- description: Delete comments.
  flows:
  - authorizationCode
  scope: delete:comment:confluence
- description: Delete content.
  flows:
  - authorizationCode
  scope: delete:content:confluence
- description: Delete custom content.
  flows:
  - authorizationCode
  scope: delete:custom-content:confluence
- description: Delete databases.
  flows:
  - authorizationCode
  scope: delete:database:confluence
- description: Delete Smart Links in the content tree.
  flows:
  - authorizationCode
  scope: delete:embed:confluence
- description: Delete folders.
  flows:
  - authorizationCode
  scope: delete:folder:confluence
- description: Delete pages.
  flows:
  - authorizationCode
  scope: delete:page:confluence
- description: Delete spaces.
  flows:
  - authorizationCode
  scope: delete:space:confluence
- description: Delete whiteboards.
  flows:
  - authorizationCode
  scope: delete:whiteboard:confluence
- description: Manage global settings.
  flows:
  - authorizationCode
  scope: manage:confluence-configuration
- description: Moderate comments
  flows:
  - authorizationCode
  scope: moderate:comment:confluence
- description: Moderate core contents
  flows:
  - authorizationCode
  scope: moderate:core-content:confluence
- description: View analytics for content.
  flows:
  - authorizationCode
  scope: read:analytics.content:confluence
- description: ''
  flows: []
  scope: read:app-data:confluence
- description: View and download content attachments.
  flows:
  - authorizationCode
  scope: read:attachment:confluence
- description: View audit records.
  flows:
  - authorizationCode
  scope: read:audit-log:confluence
- description: View blogposts.
  flows:
  - authorizationCode
  scope: read:blogpost:confluence
- description: View comments.
  flows:
  - authorizationCode
  scope: read:comment:confluence
- description: View Confluence settings.
  flows:
  - authorizationCode
  scope: read:configuration:confluence
- description: Read all content, including content body (expansions permitted). Note, APIs using this scope may also return data allowed by read:confluence-space.summary. However, this scope is not a substitute for read:confluence-space.summary.
  flows:
  - authorizationCode
  scope: read:confluence-content.all
- description: Read content permissions.
  flows:
  - authorizationCode
  scope: read:confluence-content.permission
- description: Read a summary of the content, which is the content without expansions. Note, APIs using this scope may also return data allowed by read:confluence-space.summary. However, this scope is not a substitute for read:confluence-space.summary.
  flows:
  - authorizationCode
  scope: read:confluence-content.summary
- description: Read user groups.
  flows:
  - authorizationCode
  scope: read:confluence-groups
- description: Read content properties.
  flows:
  - authorizationCode
  scope: read:confluence-props
- description: Read a summary of space information without expansions.
  flows:
  - authorizationCode
  scope: read:confluence-space.summary
- description: Read users.
  flows:
  - authorizationCode
  scope: read:confluence-user
- description: View content details.
  flows:
  - authorizationCode
  scope: read:content-details:confluence
- description: View content summaries.
  flows:
  - authorizationCode
  scope: read:content.metadata:confluence
- description: Check content permissions.
  flows:
  - authorizationCode
  scope: read:content.permission:confluence
- description: View content properties.
  flows:
  - authorizationCode
  scope: read:content.property:confluence
- description: View content restrictions.
  flows:
  - authorizationCode
  scope: read:content.restriction:confluence
- description: View content.
  flows:
  - authorizationCode
  scope: read:content:confluence
- description: View custom content.
  flows:
  - authorizationCode
  scope: read:custom-content:confluence
- description: View databases and their properties.
  flows:
  - authorizationCode
  scope: read:database:confluence
- description: View email addresses of all users regardless of the user’s profile visibility settings.
  flows:
  - authorizationCode
  scope: read:email-address:confluence
- description: View Smart Links in the content tree and their properties.
  flows:
  - authorizationCode
  scope: read:embed:confluence
- description: View folders and their properties.
  flows:
  - authorizationCode
  scope: read:folder:confluence
- description: View groups.
  flows:
  - authorizationCode
  scope: read:group:confluence
- description: View children and descendants in the content tree.
  flows:
  - authorizationCode
  scope: read:hierarchical-content:confluence
- description: View tasks.
  flows:
  - authorizationCode
  scope: read:inlinetask:confluence
- description: View labels.
  flows:
  - authorizationCode
  scope: read:label:confluence
- description: View pages.
  flows:
  - authorizationCode
  scope: read:page:confluence
- description: View entity relationships.
  flows:
  - authorizationCode
  scope: read:relation:confluence
- description: View space details.
  flows:
  - authorizationCode
  scope: read:space-details:confluence
- description: View space permissions.
  flows:
  - authorizationCode
  scope: read:space.permission:confluence
- description: View space properties.
  flows:
  - authorizationCode
  scope: read:space.property:confluence
- description: View space settings.
  flows:
  - authorizationCode
  scope: read:space.setting:confluence
- description: View spaces.
  flows:
  - authorizationCode
  scope: read:space:confluence
- description: View tasks.
  flows:
  - authorizationCode
  scope: read:task:confluence
- description: View content templates.
  flows:
  - authorizationCode
  scope: read:template:confluence
- description: View user properties.
  flows:
  - authorizationCode
  scope: read:user.property:confluence
- description: View user details.
  flows:
  - authorizationCode
  scope: read:user:confluence
- description: View content watchers.
  flows:
  - authorizationCode
  scope: read:watcher:confluence
- description: View whiteboards.
  flows:
  - authorizationCode
  scope: read:whiteboard:confluence
- description: Download attachments of a Confluence page or blogpost that you have access to.
  flows:
  - authorizationCode
  scope: readonly:content.attachment:confluence
- description: Search Confluence. Note, APIs using this scope may also return data allowed by read:confluence-space.summary and read:confluence-content.summary. However, this scope is not a substitute for read:confluence-space.summary or read:confluence-content.summary.
  flows:
  - authorizationCode
  scope: search:confluence
- description: Create, update and delete app properties.
  flows:
  - authorizationCode
  scope: write:app-data:confluence
- description: Create and update attachments.
  flows:
  - authorizationCode
  scope: write:attachment:confluence
- description: Create audit records.
  flows:
  - authorizationCode
  scope: write:audit-log:confluence
- description: Create and update blogposts.
  flows:
  - authorizationCode
  scope: write:blogpost:confluence
- description: Create and update comments.
  flows:
  - authorizationCode
  scope: write:comment:confluence
- description: Update Confluence settings.
  flows:
  - authorizationCode
  scope: write:configuration:confluence
- description: Permits the creation of pages, blogs, comments and questions.
  flows:
  - authorizationCode
  scope: write:confluence-content
- description: Upload attachments.
  flows:
  - authorizationCode
  scope: write:confluence-file
- description: Create, remove and update user groups.
  flows:
  - authorizationCode
  scope: write:confluence-groups
- description: Write content properties.
  flows:
  - authorizationCode
  scope: write:confluence-props
- description: Create, update and delete space information.
  flows:
  - authorizationCode
  scope: write:confluence-space
- description: Create, update and delete content properties.
  flows:
  - authorizationCode
  scope: write:content.property:confluence
- description: Update content restrictions.
  flows:
  - authorizationCode
  scope: write:content.restriction:confluence
- description: Create and update content.
  flows:
  - authorizationCode
  scope: write:content:confluence
- description: Create and update custom content.
  flows:
  - authorizationCode
  scope: write:custom-content:confluence
- description: Create and update databases and their properties.
  flows:
  - authorizationCode
  scope: write:database:confluence
- description: Create and update Smart Links in the content tree and their properties.
  flows:
  - authorizationCode
  scope: write:embed:confluence
- description: Create and update folders and their properties.
  flows:
  - authorizationCode
  scope: write:folder:confluence
- description: Create and delete groups.
  flows:
  - authorizationCode
  scope: write:group:confluence
- description: Update tasks.
  flows:
  - authorizationCode
  scope: write:inlinetask:confluence
- description: Add and remove labels.
  flows:
  - authorizationCode
  scope: write:label:confluence
- description: Create and update pages.
  flows:
  - authorizationCode
  scope: write:page:confluence
- description: Create and update entity relationships.
  flows:
  - authorizationCode
  scope: write:relation:confluence
- description: Update space permissions.
  flows:
  - authorizationCode
  scope: write:space.permission:confluence
- description: Create, update and delete space properties.
  flows:
  - authorizationCode
  scope: write:space.property:confluence
- description: Update space settings.
  flows:
  - authorizationCode
  scope: write:space.setting:confluence
- description: Create and update spaces.
  flows:
  - authorizationCode
  scope: write:space:confluence
- description: ''
  flows: []
  scope: write:task:confluence
- description: Create, update and delete content templates.
  flows:
  - authorizationCode
  scope: write:template:confluence
- description: Create, update and delete user properties.
  flows:
  - authorizationCode
  scope: write:user.property:confluence
- description: Add and remove content watchers.
  flows:
  - authorizationCode
  scope: write:watcher:confluence
- description: Create and update whiteboards.
  flows:
  - authorizationCode
  scope: write:whiteboard:confluence
slug: atlassian-confluence-scopes
source_filename: atlassian-confluence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/atlassian-confluence-rest-v1-openapi.json, openapi/atlassian-confluence-rest-v2-openapi.json\nschemes:\n- name: oAuthDefinitions\n  source: openapi/atlassian-confluence-rest-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: This API uses OAuth 2 with the authorizationCode grant flow.\n- name: oAuthDefinitions\n  source: openapi/atlassian-confluence-rest-v2-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n  description: This API uses OAuth 2 with the authorizationCode grant flow.\nscopes:\n- scope: delete:attachment:confluence\n  description: Delete attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n\
  - scope: delete:blogpost:confluence\n  description: Delete blogposts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: delete:comment:confluence\n  description: Delete comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:content:confluence\n  description: Delete content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: delete:custom-content:confluence\n  description: Delete custom content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:database:confluence\n  description: Delete databases.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:embed:confluence\n\
  \  description: Delete Smart Links in the content tree.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:folder:confluence\n  description: Delete folders.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:page:confluence\n  description: Delete pages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: delete:space:confluence\n  description: Delete spaces.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: delete:whiteboard:confluence\n  description: Delete whiteboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: manage:confluence-configuration\n  description: Manage\
  \ global settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: moderate:comment:confluence\n  description: Moderate comments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: moderate:core-content:confluence\n  description: Moderate core contents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:analytics.content:confluence\n  description: View analytics for content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:app-data:confluence\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:attachment:confluence\n  description: View and download content attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n\
  - scope: read:audit-log:confluence\n  description: View audit records.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:blogpost:confluence\n  description: View blogposts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:comment:confluence\n  description: View comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:configuration:confluence\n  description: View Confluence settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:confluence-content.all\n  description: Read all content, including content body (expansions permitted). Note, APIs using\n    this scope may also return data allowed by read:confluence-space.summary.\
  \ However, this\n    scope is not a substitute for read:confluence-space.summary.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-content.permission\n  description: Read content permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-content.summary\n  description: Read a summary of the content, which is the content without expansions. Note,\n    APIs using this scope may also return data allowed by read:confluence-space.summary. However,\n    this scope is not a substitute for read:confluence-space.summary.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-groups\n  description: Read user groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-props\n  description: Read content\
  \ properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-space.summary\n  description: Read a summary of space information without expansions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:confluence-user\n  description: Read users.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:content-details:confluence\n  description: View content details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:content.metadata:confluence\n  description: View content summaries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:content.permission:confluence\n  description: Check content permissions.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:content.property:confluence\n  description: View content properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:content.restriction:confluence\n  description: View content restrictions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:content:confluence\n  description: View content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:custom-content:confluence\n  description: View custom content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:database:confluence\n  description: View databases and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n\
  - scope: read:email-address:confluence\n  description: View email addresses of all users regardless of the user’s profile visibility\n    settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:embed:confluence\n  description: View Smart Links in the content tree and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:folder:confluence\n  description: View folders and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:group:confluence\n  description: View groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:hierarchical-content:confluence\n  description: View children and descendants in the content tree.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n\
  - scope: read:inlinetask:confluence\n  description: View tasks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:label:confluence\n  description: View labels.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:page:confluence\n  description: View pages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:relation:confluence\n  description: View entity relationships.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:space-details:confluence\n  description: View space details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:space.permission:confluence\n  description:\
  \ View space permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:space.property:confluence\n  description: View space properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:space.setting:confluence\n  description: View space settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:space:confluence\n  description: View spaces.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:task:confluence\n  description: View tasks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:template:confluence\n  description: View content templates.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:user.property:confluence\n  description: View user properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:user:confluence\n  description: View user details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: read:watcher:confluence\n  description: View content watchers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: read:whiteboard:confluence\n  description: View whiteboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: readonly:content.attachment:confluence\n  description: Download attachments of a Confluence page or blogpost\
  \ that you have access to.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: search:confluence\n  description: Search Confluence. Note, APIs using this scope may also return data allowed by\n    read:confluence-space.summary and read:confluence-content.summary. However, this scope is\n    not a substitute for read:confluence-space.summary or read:confluence-content.summary.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:app-data:confluence\n  description: Create, update and delete app properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:attachment:confluence\n  description: Create and update attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:audit-log:confluence\n\
  \  description: Create audit records.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:blogpost:confluence\n  description: Create and update blogposts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:comment:confluence\n  description: Create and update comments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:configuration:confluence\n  description: Update Confluence settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:confluence-content\n  description: Permits the creation of pages, blogs, comments and questions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n\
  - scope: write:confluence-file\n  description: Upload attachments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:confluence-groups\n  description: Create, remove and update user groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:confluence-props\n  description: Write content properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:confluence-space\n  description: Create, update and delete space information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:content.property:confluence\n  description: Create, update and delete content properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:content.restriction:confluence\n  description: Update\
  \ content restrictions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:content:confluence\n  description: Create and update content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:custom-content:confluence\n  description: Create and update custom content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:database:confluence\n  description: Create and update databases and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:embed:confluence\n  description: Create and update Smart Links in the content tree and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:folder:confluence\n\
  \  description: Create and update folders and their properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:group:confluence\n  description: Create and delete groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:inlinetask:confluence\n  description: Update tasks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:label:confluence\n  description: Add and remove labels.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:page:confluence\n  description: Create and update pages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:relation:confluence\n  description: Create and update entity relationships.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:space.permission:confluence\n  description: Update space permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:space.property:confluence\n  description: Create, update and delete space properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:space.setting:confluence\n  description: Update space settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:space:confluence\n  description: Create and update spaces.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:task:confluence\n  sources:\n \
  \ - openapi/atlassian-confluence-rest-v2-openapi.json\n- scope: write:template:confluence\n  description: Create, update and delete content templates.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:user.property:confluence\n  description: Create, update and delete user properties.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:watcher:confluence\n  description: Add and remove content watchers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n- scope: write:whiteboard:confluence\n  description: Create and update whiteboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/scopes/atlassian-confluence-scopes.yml
summary_line: 90 scopes · authorizationCode
tags:
- Atlassian
- Collaboration
- Content Management
- Documentation
- Knowledge-Management
- Wiki
- MCP
- GraphQL
- Agents
- Productivity
token_urls:
- https://auth.atlassian.com/oauth/token
---
