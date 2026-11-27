---
api_specs:
- filename: commareports-com-account-api-openapi.yml
  format: yaml
  label: Comma Account API
  slug: commareports-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-account-api-openapi.yml
- filename: commareports-com-assets-api-openapi.yml
  format: yaml
  label: Comma Assets API
  slug: commareports-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-assets-api-openapi.yml
- filename: commareports-com-comments-api-openapi.yml
  format: yaml
  label: Comma Comments API
  slug: commareports-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-comments-api-openapi.yml
- filename: commareports-com-connectors-api-openapi.yml
  format: yaml
  label: Comma Connectors API
  slug: commareports-com-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-connectors-api-openapi.yml
- filename: commareports-com-meta-api-openapi.yml
  format: yaml
  label: Comma Meta API
  slug: commareports-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-meta-api-openapi.yml
- filename: commareports-com-notifications-api-openapi.yml
  format: yaml
  label: Comma Notifications API
  slug: commareports-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-notifications-api-openapi.yml
- filename: commareports-com-reports-api-openapi.yml
  format: yaml
  label: Comma Reports API
  slug: commareports-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reports-api-openapi.yml
- filename: commareports-com-reviewers-api-openapi.yml
  format: yaml
  label: Comma Reviewers API
  slug: commareports-com-reviewers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviewers-api-openapi.yml
- filename: commareports-com-reviews-api-openapi.yml
  format: yaml
  label: Comma Reviews API
  slug: commareports-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviews-api-openapi.yml
- filename: commareports-com-revisions-api-openapi.yml
  format: yaml
  label: Comma Revisions API
  slug: commareports-com-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-revisions-api-openapi.yml
- filename: commareports-com-routines-api-openapi.yml
  format: yaml
  label: Comma Routines API
  slug: commareports-com-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-routines-api-openapi.yml
- filename: commareports-com-sharing-api-openapi.yml
  format: yaml
  label: Comma Sharing API
  slug: commareports-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-sharing-api-openapi.yml
- filename: commareports-com-skills-api-openapi.yml
  format: yaml
  label: Comma Skills API
  slug: commareports-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-skills-api-openapi.yml
authorization_urls: []
description: ''
docs: https://commareports.com/docs/api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Comma Scopes
name_suffix: OAuth Scopes
note: These are scopes on Comma personal API tokens (comma_sk_… Bearer), not OAuth 2.0 scopes; the API declares no oauth2 securityScheme.
overview: 'Comma publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Comma API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Comma
provider_slug: commareports-com
schemes: []
scope_count: 7
scope_names:
- reports:read
- reports:write
- comments:read
- comments:write
- routines
- connections
- sharing
scopes:
- description: List, search, and read report content, revisions, and diffs.
  flows: []
  scope: reports:read
- description: Create and edit reports; upload assets; request reviews.
  flows: []
  scope: reports:write
- description: Read comment threads and replies.
  flows: []
  scope: comments:read
- description: Post, reply to, and resolve comments.
  flows: []
  scope: comments:write
- description: Manage routines, skills, reviewers, and notifications.
  flows: []
  scope: routines
- description: Manage integrations and connectors.
  flows: []
  scope: connections
- description: Change who can access a report.
  flows: []
  scope: sharing
slug: commareports-com-scopes
source_filename: commareports-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commareports.com/docs/api-tokens\ndocs: https://commareports.com/docs/api-tokens\nnote: These are scopes on Comma personal API tokens (comma_sk_… Bearer), not OAuth 2.0 scopes; the API declares no oauth2 securityScheme.\ndefault_scopes: [reports:write, comments:write, comments:read]\nscopes:\n- name: reports:read\n  description: List, search, and read report content, revisions, and diffs.\n- name: reports:write\n  description: Create and edit reports; upload assets; request reviews.\n- name: comments:read\n  description: Read comment threads and replies.\n- name: comments:write\n  description: Post, reply to, and resolve comments.\n- name: routines\n  description: Manage routines, skills, reviewers, and notifications.\n- name: connections\n  description: Manage integrations and connectors.\n- name: sharing\n  description: Change who can access a report.\n"
source_yaml_url: https://artifacts.apis.io/commareports-com/scopes/commareports-com-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Reports
- Collaboration
- Comments
- HTML
- MCP
- AI Agents
- Data Visualization
token_bound: false
token_urls: []
---
