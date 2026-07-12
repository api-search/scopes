---
authorization_urls: []
description: ''
docs: https://api.akeneo.com/apps/authentication-and-authorization.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Akeneo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Akeneo publishes 36 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Akeneo API on a user''s behalf.


  Tokens are issued from https://{tenant}.cloud.akeneo.com/api/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Akeneo
provider_slug: akeneo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.cloud.akeneo.com/api/oauth/v1/token
  name: OAuth2ClientCredentials
  source: openapi/akeneo-openapi.yml
scope_count: 36
scope_names:
- read_products
- write_products
- delete_products
- read_catalog_structure
- write_catalog_structure
- read_attribute_options
- write_attribute_options
- read_categories
- write_categories
- read_channel_localization
- read_channel_settings
- write_channel_settings
- read_association_types
- write_association_types
- read_catalogs
- write_catalogs
- delete_catalogs
- read_asset_families
- write_asset_families
- read_assets
- write_assets
- delete_assets
- read_reference_entities
- write_reference_entities
- read_reference_entity_records
- write_reference_entity_records
- read_workflows
- read_workflow_step_assignees
- read_workflow_tasks
- write_workflow_tasks
- create_suggestions
- read_suggestions
- manage_suggestions
- openid
- profile
- email
scopes:
- description: Read products
  flows: []
  scope: read_products
- description: Write products
  flows: []
  scope: write_products
- description: Remove products
  flows: []
  scope: delete_products
- description: Read attributes, attribute groups, families and family variants
  flows: []
  scope: read_catalog_structure
- description: Write attributes, attribute groups, families and family variants
  flows: []
  scope: write_catalog_structure
- description: Read attribute options
  flows: []
  scope: read_attribute_options
- description: Write attribute options
  flows: []
  scope: write_attribute_options
- description: Read categories
  flows: []
  scope: read_categories
- description: Write categories
  flows: []
  scope: write_categories
- description: Read locales and currencies
  flows: []
  scope: read_channel_localization
- description: Read channels
  flows: []
  scope: read_channel_settings
- description: Write channels
  flows: []
  scope: write_channel_settings
- description: Read association types
  flows: []
  scope: read_association_types
- description: Write association types
  flows: []
  scope: write_association_types
- description: Read app catalogs
  flows: []
  scope: read_catalogs
- description: Write app catalogs
  flows: []
  scope: write_catalogs
- description: Remove app catalogs
  flows: []
  scope: delete_catalogs
- description: Read asset families
  flows: []
  scope: read_asset_families
- description: Write assets families
  flows: []
  scope: write_asset_families
- description: Read assets
  flows: []
  scope: read_assets
- description: Write assets
  flows: []
  scope: write_assets
- description: Remove assets
  flows: []
  scope: delete_assets
- description: Read reference entities
  flows: []
  scope: read_reference_entities
- description: Write reference entities
  flows: []
  scope: write_reference_entities
- description: Read reference entity records
  flows: []
  scope: read_reference_entity_records
- description: Write reference entity records
  flows: []
  scope: write_reference_entity_records
- description: Read workflows and their steps
  flows: []
  scope: read_workflows
- description: Read assignees for workflow steps
  flows: []
  scope: read_workflow_step_assignees
- description: Read workflow tasks
  flows: []
  scope: read_workflow_tasks
- description: Write workflow tasks
  flows: []
  scope: write_workflow_tasks
- description: Create suggestions
  flows: []
  scope: create_suggestions
- description: Read suggestions
  flows: []
  scope: read_suggestions
- description: Manage suggestions
  flows: []
  scope: manage_suggestions
- description: Read user id (authentication scope)
  flows: []
  scope: openid
- description: Read user first name and last name (from PIM user profile) (authentication scope)
  flows: []
  scope: profile
- description: Read user email (from PIM user profile) (authentication scope)
  flows: []
  scope: email
slug: akeneo-scopes
source_filename: akeneo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/akeneo-openapi.yml\ndocs: https://api.akeneo.com/apps/authentication-and-authorization.html\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/akeneo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.cloud.akeneo.com/api/oauth/v1/token\nscopes:\n- scope: read_products\n  description: Read products\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_products\n  description: Write products\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: delete_products\n  description: Remove products\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_catalog_structure\n  description: Read attributes, attribute groups, families and family variants\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_catalog_structure\n\
  \  description: Write attributes, attribute groups, families and family variants\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_attribute_options\n  description: Read attribute options\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_attribute_options\n  description: Write attribute options\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_categories\n  description: Read categories\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_categories\n  description: Write categories\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_channel_localization\n  description: Read locales and currencies\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_channel_settings\n  description: Read channels\n  sources:\n \
  \ - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_channel_settings\n  description: Write channels\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_association_types\n  description: Read association types\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_association_types\n  description: Write association types\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_catalogs\n  description: Read app catalogs\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_catalogs\n  description: Write app catalogs\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: delete_catalogs\n  description: Remove app catalogs\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_asset_families\n  description:\
  \ Read asset families\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_asset_families\n  description: Write assets families\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_assets\n  description: Read assets\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_assets\n  description: Write assets\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: delete_assets\n  description: Remove assets\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_reference_entities\n  description: Read reference entities\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_reference_entities\n  description: Write reference entities\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_reference_entity_records\n\
  \  description: Read reference entity records\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_reference_entity_records\n  description: Write reference entity records\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_workflows\n  description: Read workflows and their steps\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_workflow_step_assignees\n  description: Read assignees for workflow steps\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_workflow_tasks\n  description: Read workflow tasks\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: write_workflow_tasks\n  description: Write workflow tasks\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: create_suggestions\n  description: Create suggestions\n  sources:\n\
  \  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: read_suggestions\n  description: Read suggestions\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: manage_suggestions\n  description: Manage suggestions\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: openid\n  description: Read user id (authentication scope)\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: profile\n  description: Read user first name and last name (from PIM user profile) (authentication\n    scope)\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n- scope: email\n  description: Read user email (from PIM user profile) (authentication scope)\n  sources:\n  - https://api.akeneo.com/apps/authentication-and-authorization.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/scopes/akeneo-scopes.yml
summary_line: 36 scopes · clientCredentials
tags:
- Product Information Management
- PIM
- Product Data
- Catalog Management
- Commerce
- Retail
token_urls:
- https://{tenant}.cloud.akeneo.com/api/oauth/v1/token
---
