---
api_specs:
- filename: bombbomb-accounts-api-openapi.yml
  format: yaml
  label: BombBomb Accounts API
  slug: bombbomb-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-accounts-api-openapi.yml
- filename: bombbomb-automations-api-openapi.yml
  format: yaml
  label: BombBomb Automations API
  slug: bombbomb-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-automations-api-openapi.yml
- filename: bombbomb-contacts-api-openapi.yml
  format: yaml
  label: BombBomb Contacts API
  slug: bombbomb-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-contacts-api-openapi.yml
- filename: bombbomb-curriculum-api-openapi.yml
  format: yaml
  label: BombBomb Curriculum API
  slug: bombbomb-curriculum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-curriculum-api-openapi.yml
- filename: bombbomb-emails-api-openapi.yml
  format: yaml
  label: BombBomb Emails API
  slug: bombbomb-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-emails-api-openapi.yml
- filename: bombbomb-files-api-openapi.yml
  format: yaml
  label: BombBomb Files API
  slug: bombbomb-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-files-api-openapi.yml
- filename: bombbomb-forms-api-openapi.yml
  format: yaml
  label: BombBomb Forms API
  slug: bombbomb-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-forms-api-openapi.yml
- filename: bombbomb-integrations-api-openapi.yml
  format: yaml
  label: BombBomb Integrations API
  slug: bombbomb-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-integrations-api-openapi.yml
- filename: bombbomb-lists-api-openapi.yml
  format: yaml
  label: BombBomb Lists API
  slug: bombbomb-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-lists-api-openapi.yml
- filename: bombbomb-orders-api-openapi.yml
  format: yaml
  label: BombBomb Orders API
  slug: bombbomb-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-orders-api-openapi.yml
- filename: bombbomb-prompts-api-openapi.yml
  format: yaml
  label: BombBomb Prompts API
  slug: bombbomb-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-prompts-api-openapi.yml
- filename: bombbomb-socials-api-openapi.yml
  format: yaml
  label: BombBomb Socials API
  slug: bombbomb-socials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-socials-api-openapi.yml
- filename: bombbomb-teams-api-openapi.yml
  format: yaml
  label: BombBomb Teams API
  slug: bombbomb-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-teams-api-openapi.yml
- filename: bombbomb-users-api-openapi.yml
  format: yaml
  label: BombBomb Users API
  slug: bombbomb-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-users-api-openapi.yml
- filename: bombbomb-utilities-api-openapi.yml
  format: yaml
  label: BombBomb Utilities API
  slug: bombbomb-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-utilities-api-openapi.yml
- filename: bombbomb-videos-api-openapi.yml
  format: yaml
  label: BombBomb Videos API
  slug: bombbomb-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-videos-api-openapi.yml
- filename: bombbomb-webhooks-api-openapi.yml
  format: yaml
  label: BombBomb Webhooks API
  slug: bombbomb-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bombbomb/openapi/bombbomb-webhooks-api-openapi.yml
authorization_urls:
- https://app.bombbomb.com/auth/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: BombBomb Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BombBomb publishes 23 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BombBomb API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BombBomb
provider_slug: bombbomb
schemes:
- flows:
  - authorizationUrl: https://app.bombbomb.com/auth/authorize
    flow: implicit
  name: BBOAuth2
  source: openapi/bombbomb-openapi.yaml
scope_count: 23
scope_names:
- account:manage
- account:read
- all:manage
- all:read
- automation:manage
- automation:read
- contact:manage
- contact:read
- curriculum:manage
- curriculum:read
- email:manage
- email:read
- file:manage
- file:read
- form:manage
- form:read
- list:manage
- order:manage
- settings:manage
- team:manage
- team:read
- video:manage
- video:read
scopes:
- description: View & Manage your BombBomb account
  flows:
  - implicit
  scope: account:manage
- description: View your BombBomb account
  flows:
  - implicit
  scope: account:read
- description: View & Manage your BombBomb information
  flows:
  - implicit
  scope: all:manage
- description: View your BombBomb information
  flows:
  - implicit
  scope: all:read
- description: View & Manage your BombBomb automations
  flows:
  - implicit
  scope: automation:manage
- description: View your BombBomb automations
  flows:
  - implicit
  scope: automation:read
- description: View & Manage your BombBomb contacts
  flows:
  - implicit
  scope: contact:manage
- description: View your BombBomb contacts
  flows:
  - implicit
  scope: contact:read
- description: View & Manage your BombBomb challenges
  flows:
  - implicit
  scope: curriculum:manage
- description: View your BombBomb challenges
  flows:
  - implicit
  scope: curriculum:read
- description: View & Manage your BombBomb emails
  flows:
  - implicit
  scope: email:manage
- description: View your BombBomb emails
  flows:
  - implicit
  scope: email:read
- description: View & Manage your BombBomb files
  flows:
  - implicit
  scope: file:manage
- description: View your BombBomb files
  flows:
  - implicit
  scope: file:read
- description: View & Manage your BombBomb forms
  flows:
  - implicit
  scope: form:manage
- description: View your BombBomb forms
  flows:
  - implicit
  scope: form:read
- description: View & Manage your BombBomb lists
  flows:
  - implicit
  scope: list:manage
- description: Manage your BombBomb orders
  flows:
  - implicit
  scope: order:manage
- description: Manage your BombBomb settings
  flows:
  - implicit
  scope: settings:manage
- description: View & Manage your BombBomb teams
  flows:
  - implicit
  scope: team:manage
- description: View your BombBomb teams
  flows:
  - implicit
  scope: team:read
- description: View & Manage your BombBomb videos
  flows:
  - implicit
  scope: video:manage
- description: View your BombBomb videos
  flows:
  - implicit
  scope: video:read
slug: bombbomb-scopes
source_filename: bombbomb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/bombbomb-openapi.yaml\nschemes:\n- name: BBOAuth2\n  source: openapi/bombbomb-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://app.bombbomb.com/auth/authorize\nscopes:\n- scope: account:manage\n  description: View & Manage your BombBomb account\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: account:read\n  description: View your BombBomb account\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: all:manage\n  description: View & Manage your BombBomb information\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: all:read\n  description: View your BombBomb information\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: automation:manage\n  description: View & Manage your BombBomb automations\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: automation:read\n\
  \  description: View your BombBomb automations\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: contact:manage\n  description: View & Manage your BombBomb contacts\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: contact:read\n  description: View your BombBomb contacts\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: curriculum:manage\n  description: View & Manage your BombBomb challenges\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: curriculum:read\n  description: View your BombBomb challenges\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: email:manage\n  description: View & Manage your BombBomb emails\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: email:read\n  description: View your BombBomb emails\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: file:manage\n\
  \  description: View & Manage your BombBomb files\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: file:read\n  description: View your BombBomb files\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: form:manage\n  description: View & Manage your BombBomb forms\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: form:read\n  description: View your BombBomb forms\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: list:manage\n  description: View & Manage your BombBomb lists\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: order:manage\n  description: Manage your BombBomb orders\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: settings:manage\n  description: Manage your BombBomb settings\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: team:manage\n  description: View & Manage\
  \ your BombBomb teams\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: team:read\n  description: View your BombBomb teams\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: video:manage\n  description: View & Manage your BombBomb videos\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n- scope: video:read\n  description: View your BombBomb videos\n  flows:\n  - implicit\n  sources:\n  - openapi/bombbomb-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/bombbomb/scopes/bombbomb-scopes.yml
summary_line: 23 scopes · implicit
tags:
- Company
- Video Messaging
- Sales
- Marketing
- Human Resources
token_bound: false
token_urls: []
---
