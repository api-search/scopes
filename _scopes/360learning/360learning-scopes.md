---
api_specs:
- filename: 360learning-core-api.json
  format: json
  label: 360Learning Core API v2
  slug: 360learning-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-core-api.json
- filename: 360learning-bulk-api.json
  format: json
  label: 360Learning Bulk API v2
  slug: 360learning-bulk-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-bulk-api.json
- filename: 360learning-webhook-api.json
  format: json
  label: 360Learning Webhook API v2
  slug: 360learning-webhook-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-webhook-api.json
- filename: 360learning-plugin-api.json
  format: json
  label: 360Learning Plugin API v2
  slug: 360learning-plugin-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-plugin-api.json
- filename: 360learning-user-authorized-api.json
  format: json
  label: 360Learning User Authorized API v2
  slug: 360learning-user-authorized-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-user-authorized-api.json
authorization_urls: []
description: ''
docs: https://360learning.readme.io/docs/oauth-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: 360Learning Scopes
name_suffix: OAuth Scopes
note: ''
overview: '360Learning publishes 45 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the 360Learning API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 360Learning
provider_slug: 360learning
schemes:
- grant: client_credentials
  name: oauth2
  sources:
  - openapi/360learning-bulk-api.json
  - openapi/360learning-core-api.json
  - openapi/360learning-plugin-api.json
  - openapi/360learning-user-authorized-api.json
  - openapi/360learning-webhook-api.json
  tokenUrl: https://app.360learning.com/api/v2/oauth2/token
  type: oauth2
scope_count: 45
scope_names:
- attendanceSheets:read
- attendanceSheets:write
- bulkOperations:read
- certificateOutlines:read
- certificateOutlines:write
- classrooms:read
- classrooms:write
- courseStats:read
- courses:read
- courses:write
- customFields:read
- customFields:write
- customLinks:read
- customLinks:write
- externalIds:read
- externalIds:write
- groups:bulk
- groups:read
- groups:write
- integrations:bulk
- integrations:read
- integrations:write
- learningNeeds:read
- pathStats:read
- paths:read
- paths:write
- projects:read
- skills:bulk
- skills:read
- skillsJobSkills:bulk
- skillsJobs:bulk
- skillsJobs:write
- skillsLibraries:bulk
- skillsPowers:bulk
- skillsPowers:read
- subscriptions:bulk
- tags:read
- tags:write
- tokens:write
- users:read
- users:write
- webhookSecrets:read
- webhookSecrets:write
- webhooks:read
- webhooks:write
scopes:
- description: Read (retrieve) access to attendance sheets.
  flows: []
  scope: attendanceSheets:read
- description: Create, update, or delete access to attendance sheets.
  flows: []
  scope: attendanceSheets:write
- description: Read (retrieve) access to bulk operations.
  flows: []
  scope: bulkOperations:read
- description: Read (retrieve) access to certificate outlines.
  flows: []
  scope: certificateOutlines:read
- description: Create, update, or delete access to certificate outlines.
  flows: []
  scope: certificateOutlines:write
- description: Read (retrieve) access to classrooms.
  flows: []
  scope: classrooms:read
- description: Create, update, or delete access to classrooms.
  flows: []
  scope: classrooms:write
- description: Read (retrieve) access to course stats.
  flows: []
  scope: courseStats:read
- description: Read (retrieve) access to courses.
  flows: []
  scope: courses:read
- description: Create, update, or delete access to courses.
  flows: []
  scope: courses:write
- description: Read (retrieve) access to custom fields.
  flows: []
  scope: customFields:read
- description: Create, update, or delete access to custom fields.
  flows: []
  scope: customFields:write
- description: Read (retrieve) access to custom links.
  flows: []
  scope: customLinks:read
- description: Create, update, or delete access to custom links.
  flows: []
  scope: customLinks:write
- description: Read (retrieve) access to external ids.
  flows: []
  scope: externalIds:read
- description: Create, update, or delete access to external ids.
  flows: []
  scope: externalIds:write
- description: Bulk operations on groups.
  flows: []
  scope: groups:bulk
- description: Read (retrieve) access to groups.
  flows: []
  scope: groups:read
- description: Create, update, or delete access to groups.
  flows: []
  scope: groups:write
- description: Bulk operations on integrations.
  flows: []
  scope: integrations:bulk
- description: Read (retrieve) access to integrations.
  flows: []
  scope: integrations:read
- description: Create, update, or delete access to integrations.
  flows: []
  scope: integrations:write
- description: Read (retrieve) access to learning needs.
  flows: []
  scope: learningNeeds:read
- description: Read (retrieve) access to path stats.
  flows: []
  scope: pathStats:read
- description: Read (retrieve) access to paths.
  flows: []
  scope: paths:read
- description: Create, update, or delete access to paths.
  flows: []
  scope: paths:write
- description: Read (retrieve) access to projects.
  flows: []
  scope: projects:read
- description: Bulk operations on skills.
  flows: []
  scope: skills:bulk
- description: Read (retrieve) access to skills.
  flows: []
  scope: skills:read
- description: Bulk operations on skills job skills.
  flows: []
  scope: skillsJobSkills:bulk
- description: Bulk operations on skills jobs.
  flows: []
  scope: skillsJobs:bulk
- description: Create, update, or delete access to skills jobs.
  flows: []
  scope: skillsJobs:write
- description: Bulk operations on skills libraries.
  flows: []
  scope: skillsLibraries:bulk
- description: Bulk operations on skills powers.
  flows: []
  scope: skillsPowers:bulk
- description: Read (retrieve) access to skills powers.
  flows: []
  scope: skillsPowers:read
- description: Bulk operations on subscriptions.
  flows: []
  scope: subscriptions:bulk
- description: Read (retrieve) access to tags.
  flows: []
  scope: tags:read
- description: Create, update, or delete access to tags.
  flows: []
  scope: tags:write
- description: Create, update, or delete access to tokens.
  flows: []
  scope: tokens:write
- description: Read (retrieve) access to users.
  flows: []
  scope: users:read
- description: Create, update, or delete access to users.
  flows: []
  scope: users:write
- description: Read (retrieve) access to webhook secrets.
  flows: []
  scope: webhookSecrets:read
- description: Create, update, or delete access to webhook secrets.
  flows: []
  scope: webhookSecrets:write
- description: Read (retrieve) access to webhooks.
  flows: []
  scope: webhooks:read
- description: Create, update, or delete access to webhooks.
  flows: []
  scope: webhooks:write
slug: 360learning-scopes
source_filename: 360learning-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/360learning-core-api.json (operation descriptions)\ndocs: https://360learning.readme.io/docs/oauth-scopes\nnotes: >-\n  Scopes follow a resource:action format. action is read (retrieve), write\n  (create/update/delete), or bulk (bulk operations). Scopes operate at two\n  levels: company-level (the permission ceiling, changed via Customer Success\n  Partner) and credential-level (a subset assigned per API credential).\n  The 360Learning OpenAPI declares an oauth2 scheme with empty flows; the\n  scope each endpoint requires is documented in its operation description and\n  enforced at request time (403 invalid_scope on failure).\nschemes:\n- name: oauth2\n  type: oauth2\n  grant: client_credentials\n  tokenUrl: https://app.360learning.com/api/v2/oauth2/token\n  sources:\n  - openapi/360learning-bulk-api.json\n  - openapi/360learning-core-api.json\n  - openapi/360learning-plugin-api.json\n  - openapi/360learning-user-authorized-api.json\n\
  \  - openapi/360learning-webhook-api.json\nscopes:\n- scope: attendanceSheets:read\n  description: Read (retrieve) access to attendance sheets.\n  sources: [openapi/360learning-core-api.json]\n- scope: attendanceSheets:write\n  description: Create, update, or delete access to attendance sheets.\n  sources: [openapi/360learning-core-api.json]\n- scope: bulkOperations:read\n  description: Read (retrieve) access to bulk operations.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: certificateOutlines:read\n  description: Read (retrieve) access to certificate outlines.\n  sources: [openapi/360learning-core-api.json]\n- scope: certificateOutlines:write\n  description: Create, update, or delete access to certificate outlines.\n  sources: [openapi/360learning-core-api.json]\n- scope: classrooms:read\n  description: Read (retrieve) access to classrooms.\n  sources: [openapi/360learning-core-api.json]\n- scope: classrooms:write\n  description: Create, update, or delete access to classrooms.\n\
  \  sources: [openapi/360learning-core-api.json]\n- scope: courseStats:read\n  description: Read (retrieve) access to course stats.\n  sources: [openapi/360learning-core-api.json]\n- scope: courses:read\n  description: Read (retrieve) access to courses.\n  sources: [openapi/360learning-core-api.json]\n- scope: courses:write\n  description: Create, update, or delete access to courses.\n  sources: [openapi/360learning-core-api.json]\n- scope: customFields:read\n  description: Read (retrieve) access to custom fields.\n  sources: [openapi/360learning-core-api.json]\n- scope: customFields:write\n  description: Create, update, or delete access to custom fields.\n  sources: [openapi/360learning-core-api.json]\n- scope: customLinks:read\n  description: Read (retrieve) access to custom links.\n  sources: [openapi/360learning-core-api.json]\n- scope: customLinks:write\n  description: Create, update, or delete access to custom links.\n  sources: [openapi/360learning-core-api.json]\n- scope: externalIds:read\n\
  \  description: Read (retrieve) access to external ids.\n  sources: [openapi/360learning-core-api.json]\n- scope: externalIds:write\n  description: Create, update, or delete access to external ids.\n  sources: [openapi/360learning-core-api.json]\n- scope: groups:bulk\n  description: Bulk operations on groups.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: groups:read\n  description: Read (retrieve) access to groups.\n  sources: [openapi/360learning-core-api.json]\n- scope: groups:write\n  description: Create, update, or delete access to groups.\n  sources: [openapi/360learning-core-api.json]\n- scope: integrations:bulk\n  description: Bulk operations on integrations.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: integrations:read\n  description: Read (retrieve) access to integrations.\n  sources: [openapi/360learning-core-api.json]\n- scope: integrations:write\n  description: Create, update, or delete access to integrations.\n  sources: [openapi/360learning-core-api.json]\n\
  - scope: learningNeeds:read\n  description: Read (retrieve) access to learning needs.\n  sources: [openapi/360learning-core-api.json]\n- scope: pathStats:read\n  description: Read (retrieve) access to path stats.\n  sources: [openapi/360learning-core-api.json]\n- scope: paths:read\n  description: Read (retrieve) access to paths.\n  sources: [openapi/360learning-core-api.json]\n- scope: paths:write\n  description: Create, update, or delete access to paths.\n  sources: [openapi/360learning-core-api.json]\n- scope: projects:read\n  description: Read (retrieve) access to projects.\n  sources: [openapi/360learning-core-api.json]\n- scope: skills:bulk\n  description: Bulk operations on skills.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: skills:read\n  description: Read (retrieve) access to skills.\n  sources: [openapi/360learning-core-api.json]\n- scope: skillsJobSkills:bulk\n  description: Bulk operations on skills job skills.\n  sources: [openapi/360learning-bulk-api.json]\n\
  - scope: skillsJobs:bulk\n  description: Bulk operations on skills jobs.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: skillsJobs:write\n  description: Create, update, or delete access to skills jobs.\n  sources: [openapi/360learning-core-api.json]\n- scope: skillsLibraries:bulk\n  description: Bulk operations on skills libraries.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: skillsPowers:bulk\n  description: Bulk operations on skills powers.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: skillsPowers:read\n  description: Read (retrieve) access to skills powers.\n  sources: [openapi/360learning-core-api.json]\n- scope: subscriptions:bulk\n  description: Bulk operations on subscriptions.\n  sources: [openapi/360learning-bulk-api.json]\n- scope: tags:read\n  description: Read (retrieve) access to tags.\n  sources: [openapi/360learning-core-api.json]\n- scope: tags:write\n  description: Create, update, or delete access to tags.\n  sources: [openapi/360learning-core-api.json]\n\
  - scope: tokens:write\n  description: Create, update, or delete access to tokens.\n  sources: [openapi/360learning-core-api.json]\n- scope: users:read\n  description: Read (retrieve) access to users.\n  sources: [openapi/360learning-core-api.json, openapi/360learning-user-authorized-api.json]\n- scope: users:write\n  description: Create, update, or delete access to users.\n  sources: [openapi/360learning-core-api.json]\n- scope: webhookSecrets:read\n  description: Read (retrieve) access to webhook secrets.\n  sources: [openapi/360learning-webhook-api.json]\n- scope: webhookSecrets:write\n  description: Create, update, or delete access to webhook secrets.\n  sources: [openapi/360learning-webhook-api.json]\n- scope: webhooks:read\n  description: Read (retrieve) access to webhooks.\n  sources: [openapi/360learning-webhook-api.json]\n- scope: webhooks:write\n  description: Create, update, or delete access to webhooks.\n  sources: [openapi/360learning-webhook-api.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/scopes/360learning-scopes.yml
summary_line: 45 scopes
tags:
- Company
- Edtech
- Learning Management System
- E-Learning
- Training
- Collaborative Learning
- HR Tech
- Skills
- API
token_urls: []
---
