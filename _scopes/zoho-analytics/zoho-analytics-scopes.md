---
api_specs:
- filename: analytics-oas
  format: yaml
  label: Zoho Analytics API
  slug: zoho-analytics-api
  spec_type: OpenAPI
  url: https://github.com/zoho/analytics-oas
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Analytics publishes 31 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Analytics API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Analytics
provider_slug: zoho-analytics
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/bulk-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/data-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/embed-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/metadata-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/modeling-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/share-api.json
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  source: openapi/usermanagement-api.json
scope_count: 31
scope_names:
- ZohoAnalytics.data.all
- ZohoAnalytics.data.create
- ZohoAnalytics.data.delete
- ZohoAnalytics.data.read
- ZohoAnalytics.data.update
- ZohoAnalytics.embed.all
- ZohoAnalytics.embed.create
- ZohoAnalytics.embed.delete
- ZohoAnalytics.embed.read
- ZohoAnalytics.embed.update
- ZohoAnalytics.fullaccess.all
- ZohoAnalytics.metadata.all
- ZohoAnalytics.metadata.create
- ZohoAnalytics.metadata.delete
- ZohoAnalytics.metadata.read
- ZohoAnalytics.metadata.update
- ZohoAnalytics.modeling.all
- ZohoAnalytics.modeling.create
- ZohoAnalytics.modeling.delete
- ZohoAnalytics.modeling.read
- ZohoAnalytics.modeling.update
- ZohoAnalytics.share.all
- ZohoAnalytics.share.create
- ZohoAnalytics.share.delete
- ZohoAnalytics.share.read
- ZohoAnalytics.share.update
- ZohoAnalytics.usermanagement.all
- ZohoAnalytics.usermanagement.create
- ZohoAnalytics.usermanagement.delete
- ZohoAnalytics.usermanagement.read
- ZohoAnalytics.usermanagement.update
scopes:
- description: Full access to data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.data.all
- description: Create data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.data.create
- description: Delete data from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.data.delete
- description: Read data from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.data.read
- description: Update data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.data.update
- description: Full access to embedded content in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.embed.all
- description: Create embedded content in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.embed.create
- description: De;lete embedded content from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.embed.delete
- description: Read embedded content from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.embed.read
- description: Update embedded content in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.embed.update
- description: Full access to all Zoho Analytics features.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.fullaccess.all
- description: Full access to metadata in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.metadata.all
- description: Create metadata resource in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.metadata.create
- description: Delete metadata resource from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.metadata.delete
- description: Read metadata resource from Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.metadata.read
- description: Update metadata resource in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.metadata.update
- description: Full access to modeling objects in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.modeling.all
- description: Create modeling objects in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.modeling.create
- description: Delete modeling objects in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.modeling.delete
- description: ''
  flows: []
  scope: ZohoAnalytics.modeling.read
- description: Update modeling objects in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.modeling.update
- description: Full access to shared items in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.share.all
- description: Create shared items in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.share.create
- description: Delete shared items in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.share.delete
- description: Read shared items in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.share.read
- description: Update shared items in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.share.update
- description: Full access to user management in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.usermanagement.all
- description: Create user management data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.usermanagement.create
- description: Delete user management data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.usermanagement.delete
- description: Read user management data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.usermanagement.read
- description: Update user management data in Zoho Analytics.
  flows:
  - authorizationCode
  scope: ZohoAnalytics.usermanagement.update
slug: zoho-analytics-scopes
source_filename: zoho-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bulk-api.json, openapi/data-api.json, openapi/embed-api.json, openapi/metadata-api.json,\n  openapi/modeling-api.json, openapi/share-api.json, openapi/usermanagement-api.json\nschemes:\n- name: iam-oauth2-schema\n  source: openapi/bulk-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/data-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/embed-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/metadata-api.json\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/modeling-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/share-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n- name: iam-oauth2-schema\n  source: openapi/usermanagement-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n- scope: ZohoAnalytics.data.all\n  description: Full access to data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n- scope: ZohoAnalytics.data.create\n\
  \  description: Create data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n- scope: ZohoAnalytics.data.delete\n  description: Delete data from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n- scope: ZohoAnalytics.data.read\n  description: Read data from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n- scope: ZohoAnalytics.data.update\n  description: Update data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n- scope: ZohoAnalytics.embed.all\n  description: Full access to embedded content in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/embed-api.json\n- scope: ZohoAnalytics.embed.create\n  description: Create embedded content in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/embed-api.json\n- scope: ZohoAnalytics.embed.delete\n  description: De;lete embedded content from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/embed-api.json\n- scope: ZohoAnalytics.embed.read\n  description: Read embedded content from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/embed-api.json\n- scope: ZohoAnalytics.embed.update\n  description: Update embedded content in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/embed-api.json\n- scope: ZohoAnalytics.fullaccess.all\n  description: Full access to all Zoho Analytics features.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n  - openapi/embed-api.json\n  - openapi/metadata-api.json\n  - openapi/modeling-api.json\n  - openapi/share-api.json\n  - openapi/usermanagement-api.json\n- scope: ZohoAnalytics.metadata.all\n  description: Full access to metadata in Zoho Analytics.\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/metadata-api.json\n- scope: ZohoAnalytics.metadata.create\n  description: Create metadata resource in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/metadata-api.json\n- scope: ZohoAnalytics.metadata.delete\n  description: Delete metadata resource from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/metadata-api.json\n- scope: ZohoAnalytics.metadata.read\n  description: Read metadata resource from Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/metadata-api.json\n- scope: ZohoAnalytics.metadata.update\n  description: Update metadata resource in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/metadata-api.json\n- scope: ZohoAnalytics.modeling.all\n  description: Full access to modeling objects in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/modeling-api.json\n- scope: ZohoAnalytics.modeling.create\n  description:\
  \ Create modeling objects in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/modeling-api.json\n- scope: ZohoAnalytics.modeling.delete\n  description: Delete modeling objects in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/modeling-api.json\n- scope: ZohoAnalytics.modeling.read\n  sources:\n  - openapi/modeling-api.json\n- scope: ZohoAnalytics.modeling.update\n  description: Update modeling objects in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/modeling-api.json\n- scope: ZohoAnalytics.share.all\n  description: Full access to shared items in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/share-api.json\n- scope: ZohoAnalytics.share.create\n  description: Create shared items in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/share-api.json\n- scope: ZohoAnalytics.share.delete\n  description: Delete shared items in Zoho Analytics.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/share-api.json\n- scope: ZohoAnalytics.share.read\n  description: Read shared items in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/share-api.json\n- scope: ZohoAnalytics.share.update\n  description: Update shared items in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/share-api.json\n- scope: ZohoAnalytics.usermanagement.all\n  description: Full access to user management in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usermanagement-api.json\n- scope: ZohoAnalytics.usermanagement.create\n  description: Create user management data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usermanagement-api.json\n- scope: ZohoAnalytics.usermanagement.delete\n  description: Delete user management data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usermanagement-api.json\n- scope: ZohoAnalytics.usermanagement.read\n  description: Read\
  \ user management data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usermanagement-api.json\n- scope: ZohoAnalytics.usermanagement.update\n  description: Update user management data in Zoho Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usermanagement-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-analytics/refs/heads/main/scopes/zoho-analytics-scopes.yml
summary_line: 31 scopes · authorizationCode
tags:
- Business Intelligence
- Analytics
- Dashboards
- Reports
- Data Import
- Data Export
- Workspaces
- Visualizations
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
