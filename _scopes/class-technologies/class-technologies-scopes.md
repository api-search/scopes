---
authorization_urls: []
description: ''
docs: https://developer.class.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Class Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Class Technologies publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Class Technologies API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Class Technologies
provider_slug: class-technologies
schemes:
- name: apiKeyBearer
  scheme: bearer
  source: https://developer.class.com/
  type: http
scope_count: 12
scope_names:
- class:read
- class:write
- enrollment:read
- enrollment:write
- attendance:read
- metrics:read
- schedule:read
- schedule:write
- template:read
- template:write
- user:read
- user:write
scopes:
- description: Read class information.
  flows: []
  scope: class:read
- description: Create and modify classes.
  flows: []
  scope: class:write
- description: Read enrollment data.
  flows: []
  scope: enrollment:read
- description: Create and modify enrollments.
  flows: []
  scope: enrollment:write
- description: Access attendance reports.
  flows: []
  scope: attendance:read
- description: Retrieve activity and engagement metrics.
  flows: []
  scope: metrics:read
- description: View class schedules.
  flows: []
  scope: schedule:read
- description: Add or remove class dates and modify schedules.
  flows: []
  scope: schedule:write
- description: Read template information.
  flows: []
  scope: template:read
- description: Create and modify reusable class templates.
  flows: []
  scope: template:write
- description: Read user data.
  flows: []
  scope: user:read
- description: Create and modify non-learner users (admins, instructors).
  flows: []
  scope: user:write
slug: class-technologies-scopes
source_filename: class-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.class.com/\ndocs: https://developer.class.com/\nmodel: api-key-scopes\nnotes: >-\n  Class scopes are attached to API-key secrets (not an OAuth2 authorization flow).\n  Each endpoint requires one or more scopes; a request whose key lacks a required\n  scope returns HTTP 403.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  source: https://developer.class.com/\nscopes:\n- scope: class:read\n  description: Read class information.\n- scope: class:write\n  description: Create and modify classes.\n- scope: enrollment:read\n  description: Read enrollment data.\n- scope: enrollment:write\n  description: Create and modify enrollments.\n- scope: attendance:read\n  description: Access attendance reports.\n- scope: metrics:read\n  description: Retrieve activity and engagement metrics.\n- scope: schedule:read\n  description: View class schedules.\n- scope: schedule:write\n  description: Add or remove\
  \ class dates and modify schedules.\n- scope: template:read\n  description: Read template information.\n- scope: template:write\n  description: Create and modify reusable class templates.\n- scope: user:read\n  description: Read user data.\n- scope: user:write\n  description: Create and modify non-learner users (admins, instructors).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class-technologies/refs/heads/main/scopes/class-technologies-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Edtech
- Education
- Virtual Classroom
- E-Learning
- LMS
- Online Learning
- Corporate Training
- Video Conferencing
token_urls: []
---
