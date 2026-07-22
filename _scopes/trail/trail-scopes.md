---
api_specs:
- filename: trail_task_reports_v1.yaml
  format: yaml
  label: Trail Task Reports API
  slug: trail-task-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_reports_v1.yaml
- filename: trail_task_instances_v1.yaml
  format: yaml
  label: Trail Task Instances API
  slug: trail-task-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_instances_v1.yaml
- filename: trail_task_templates_v1.yaml
  format: yaml
  label: Trail Task Templates API
  slug: trail-task-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_templates_v1.yaml
- filename: trail_sites_v1.yaml
  format: yaml
  label: Trail Sites API
  slug: trail-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_sites_v1.yaml
- filename: trail_areas_v1.yaml
  format: yaml
  label: Trail Areas API
  slug: trail-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_areas_v1.yaml
- filename: trail_tags_v1.yaml
  format: yaml
  label: Trail Tags API
  slug: trail-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_tags_v1.yaml
- filename: trail_scores_v1.yaml
  format: yaml
  label: Trail Scores API
  slug: trail-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_scores_v1.yaml
- filename: trail_evo_api_v1.yaml
  format: yaml
  label: Trail Evo API
  slug: trail-evo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_evo_api_v1.yaml
authorization_urls:
- https://preprodidentity.accessacloud.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Trail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trail publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trail API on a user''s behalf.


  Tokens are issued from /api/evo_api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trail
provider_slug: trail
schemes:
- flows:
  - authorizationUrl: https://preprodidentity.accessacloud.com/connect/authorize
    flow: authorizationCode
    tokenUrl: /api/evo_api/oauth/token
  name: oauth2
  source: openapi/trail_evo_api_v1.yaml
scope_count: 4
scope_names:
- access.trail.api
- email
- openid
- profile
scopes:
- description: Trail API
  flows:
  - authorizationCode
  scope: access.trail.api
- description: Email
  flows:
  - authorizationCode
  scope: email
- description: OpenID
  flows:
  - authorizationCode
  scope: openid
- description: Profile
  flows:
  - authorizationCode
  scope: profile
slug: trail-scopes
source_filename: trail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/trail_evo_api_v1.yaml\nschemes:\n- name: oauth2\n  source: openapi/trail_evo_api_v1.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://preprodidentity.accessacloud.com/connect/authorize\n    tokenUrl: /api/evo_api/oauth/token\nscopes:\n- scope: access.trail.api\n  description: Trail API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trail_evo_api_v1.yaml\n- scope: email\n  description: Email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trail_evo_api_v1.yaml\n- scope: openid\n  description: OpenID\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trail_evo_api_v1.yaml\n- scope: profile\n  description: Profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trail_evo_api_v1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/scopes/trail-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Hospitality
- Checklists
- Task Management
- Compliance
- Food Safety
- Operations
token_urls:
- /api/evo_api/oauth/token
---
